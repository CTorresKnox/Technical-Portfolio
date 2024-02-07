# Video Game Recommendation Application - RShiny 
Online Link: https://chrizt3.shinyapps.io/VideoGameRecommender/
## About
blah

## Setup & UI Code
```
library(shiny)
library(shinyWidgets)
library(arules)
library(dplyr)
load("Movies-RawData.RData")

ui <- fluidPage(
  titlePanel(title=div(img(src="gems.png"), "Hidden Gems Movie Recommender")),
  sidebarLayout(
    sidebarPanel(
      selectInput("movies", "Select a movie:",
                  choices = sort(POPULARITY$title),
                  multiple = TRUE,
                  selected = c("Mulholland Drive (2001)", "Memento (2000)", "Inception (2010)", 
                               "Donnie Darko (2001)","Black Swan (2010)","Primer (2004)",
                               "Triangle (2009)","Midsommar (2019)","Predestination (2014)",
                               "Game, The (1997)","Cube (1997)","Creep (2014)")
                ),
      sliderInput("num_recs", "How many recs:", min = 1, max = 20, value = 5),
      sliderInput("confidence", "How confident:", min = 1, max = 100, value = 50),
      submitButton("Give me movies!", icon = icon("movie"), )
    ),
    mainPanel(
      DT::dataTableOutput("rec_table")
    )
  )
)
```

## Server Code 
```
server <- function(input, output, session) {
  output$rec_table <- DT::renderDataTable({
    movies <- 
    
    movies.too.popular <- POPULARITY$title[which(POPULARITY$popularity > .75)] # Hunt for super obscure games played by <= 0.75% of players
    
    dont.recommend <- setdiff(movies.too.popular, input$movies)
  
    RULES <- apriori(TRANS,
                     parameter = list(supp = 5 / length(TRANS), conf = input$confidence / 100, minlen = 2, maxtime = 0),
                     appearance = list(none = dont.recommend, lhs = input$movie, default = "rhs"),
                     control = list(verbose = FALSE)
    )
    
   
    RULES <- RULES[is.significant(RULES, TRANS)]
    req(length(RULES))
    RULESDF <- DATAFRAME(RULES, separate = TRUE, setStart = "", itemSep = " + ", setEnd = "")
    
   
    legit.recommendations <- setdiff(RULESDF$RHS, input$movies) # In RHS but not in input list of games
    RULESDF <- RULESDF %>% filter(RHS %in% legit.recommendations)
    
    

    RECS <- RULESDF %>%
      group_by(RHS) %>%
      summarize(Confidence = max(confidence))
    
   
    RESULTS <- RECS %>%
      left_join(POPULARITY, by = c("RHS" = "title")) %>%
      arrange(desc(Confidence))
    names(RESULTS) <- c("Game", "Confidence", "PercentPlayed")
  
    row.names(RESULTS) <- NULL
    head(RESULTS, input$num_recs)
    
  })
}

shinyApp(ui, server)
```
