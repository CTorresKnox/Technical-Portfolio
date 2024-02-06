# AUTOMATION WITH LOOPS
Completed by Christopher Torres during the Spring of 2023. The purpose was to strengthen my skills with "for" and "while" loops while also generating useful tools.
## Banking Loop - Compound Interest 
The following "for" loop was intended to be a simple way for a person to predict their investments over time. 
### CODE

```{r LOOP 1 BANKING}

INPUT1=readline(prompt = "PLEASE ENTER THE AMOUNT OF MONEY YOU WOULD LIKE TO INVEST: $ ")
INPUT2=readline(prompt = "PLEASE ENTER THE AMOUNT OF TIME YOU PLAN ON INVESTING YOUR MONEY FOR (IN YEARS): ")
INPUT3=readline(prompt = "PLEASE ENTER THE INTREST RATE OF YOUR INVESTMENT (AS A DECIMAL BETWEEN 0 AND 1): ")



IA=as.numeric(INPUT1)
Time=as.numeric(INPUT2)
rate=as.numeric(INPUT3)

TotalAmount <- c()
T <- 1:Time

for (i in Time) {
  TotalAmount <- IA*(1+rate/1)^T*1
 
  if(rate>1) {
    stop("THE INTEREST RATE ENTERED IS GREATER THAN 1. PLEASE ENTER AN INTEREST RATE AS A DECIMAL BETWEEN 0 AND 1")
  }
  if (is.na(IA)|is.na(Time)|is.na(rate)) {
    stop("INPUT INVALID. PLEASE ONLY INPUT NUMBERS")
}
}
plot(TotalAmount,type = "l", col = "green", xlab = "Time(Years)", ylab = "Account Amount($)", main = "Investment Account Projections")
cat("YOUR INITIAL AMOUNT INVESTED OF $",(IA),"WHICH HAS BEEN INVESTED BY THE BANK FOR",(Time),"YEARS,COMPOUNDED ANNUALLY, AT AN INTEREST RATE OF",(rate),"HAS GROWN TO THE AMOUNT OF $",(TotalAmount[Time]))
```

### USER GUIDE & OUTPUT
The loop works by receiving your inputs of information and then calculating your investment growth with a compound interest formula. The loop continues to calculate your projections until it has reached the maximum time parameters provided by the user. The loop is also programmed to report a graph showing an increase in profits and a confirmation statement describing the future investment value.

*🔢STEP:1*

This loop can be started by clicking run in the top right corner of the loop 1 chunk.

![US0](https://github.com/CTorresKnox/New/assets/144376690/ced82b53-3cb9-4af4-8eff-9bad00a8aeb8)

*🔢STEP:2*

Next you should look at the CONSOLE  on the bottom of your screen where a prompt will be displayed. For the first prompt you will enter the amount desired to be invested. EX. '1000=$1,000'

![US1](https://github.com/CTorresKnox/New/assets/144376690/470ac90d-23c8-43e4-826d-804c2c55a0fc)


*🔢STEP:3*

For the second prompt you will enter the amount of time you want your money to be retired for.(in years) EX. '5=5yrs'

![US2](https://github.com/CTorresKnox/New/assets/144376690/0a9e23ed-fee4-44c2-8a5a-83dca142ad38)

*🔢STEP:4*

For the third prompt you will enter the interest ratefor your investment as a decimal.(between 0-1) EX. '.05=5%'

![US3](https://github.com/CTorresKnox/New/assets/144376690/a619efa0-6122-4b16-9559-f65afc644685)

*🔢STEP:5*

Once all prompts are answered, the loop should automatically calculate your future investment amount and display your chart.

![Output](https://github.com/CTorresKnox/New/assets/144376690/d7da31c2-7e3a-4b2a-a7db-b7ef396a1e55)

A summary will also be generated to explain your investment.

![US5](https://github.com/CTorresKnox/New/assets/144376690/29ab93dc-11e5-4311-82a7-76a9312e0fbd)


## CAR PAYMENT LOOP - Monthly Car Loan Payments with Interest
This "while" loop was intended for users to find out how long it will take them to pay off their car payments. 
### CODE
```{r}

calculateRemainingBalance <- function(principal, monthlyPayment, interestRate) {
  monthlyInterestRate <- interestRate / 12 / 100
  interestPayment <- principal * monthlyInterestRate
  principalPayment <- monthlyPayment - interestPayment
  remainingBalance <- principal - principalPayment
  return(remainingBalance)
}


calculateMonthsToPayOff <- function(loanAmount, monthlyPayment, interestRate) {
  months <- 0
  remainingBalance <- loanAmount
  
  while (remainingBalance > 0) {
    remainingBalance <- calculateRemainingBalance(remainingBalance, monthlyPayment, interestRate)
    months <- months + 1
  }
  
  return(months)
}


loanAmount <- as.numeric(readline("Enter the car loan amount: "))
monthlyPayment <- as.numeric(readline("Enter the monthly car loan payment amount: "))
interestRate <- as.numeric(readline("Enter the annual interest rate on the loan (%): "))


monthsToPayOff <- calculateMonthsToPayOff(loanAmount, monthlyPayment, interestRate)
cat("It will take", monthsToPayOff, "months to pay off the car loan.\n")
```

### USER GUIDE & OUTPUT
It works by receiving loan information such as: loan amount, interest rate, and monthly payment amount. With this information the loop calculates how long it will take for your loan amount to equal zero.It will then generate a summary recapping your loan payments.

*🔢STEP:1*

This loop can be started by clicking run in the top right corner of the loop 2 chunk.

![US0](https://github.com/CTorresKnox/New/assets/144376690/0bbe7c7e-c3d8-4cbd-8186-0bfd73e35c10)


*🔢STEP:2*

Next you should look at the "Console"  on the bottom of your screen where a prompt will be displayed. For the first prompt you will Enter the amount of your car loan. EX. '10000=$10,000'

![ST1](https://github.com/CTorresKnox/New/assets/144376690/3e730a58-816a-4368-8ffa-abcac2615a78)


*🔢STEP:3*

For the second prompt you will Enter your monthly payment amount. EX. '400=$400'

![ST2](https://github.com/CTorresKnox/New/assets/144376690/6b9a1c43-d4cd-4564-be12-097e67ca97ac)


*🔢STEP:4*

For the third prompt you will Enter the interest rate on your car loan as a percentage. EX. '5=5%'

![ST3](https://github.com/CTorresKnox/New/assets/144376690/02b24316-b250-4f23-809d-ae0776d4a52e)


*🔢STEP:5*

Once all prompts are answered, the loop should automatically calculate how many months it will take to completly pay off your car loan, and a summary will be generated to explain

![ST5](https://github.com/CTorresKnox/New/assets/144376690/b82d2a98-7a07-4feb-9e28-8bbe13142721)



