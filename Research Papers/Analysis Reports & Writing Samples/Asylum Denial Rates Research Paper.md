## Asylum Denial Rates Research Project 
Deliverable: [Torres,Christopher Final Project.pdf](https://github.com/user-attachments/files/16016280/Torres.Christopher.Final.Project.pdf)

# <p align="center"> THE RELATIONSHIP BETWEEN CHARACTERISTIC DIFFERENCES OF IMMIGRATION COURT JUDGES AND ASLYLUM DENIAL RATES IN THE UNITED STATES
<p align="center"> Christopher Torres


<p align="center"> Research Project
<p align="center"> December 2023
<p align="center">ECON 381
  
## <p align="center"> ABSTRACT
The United States immigration courts recently approved a historically large amount of asylum seekers cases in 2022, but the years leading up saw some of the largest denial rates ever. The fate of asylum seekers has been historically shaped by the attributes of the immigration judge assigned to adjudicate their case, yet the denial rates between judges have serious variation. I used individual judge denial rates and descriptive characteristics to formulate a panel dataset to explore whether specific traits in judges increase asylum denial rates. I found certain characteristics such as the political affiliation of their state and the sex of the judge to be the main drivers increasing denial rates, but our model could not find any statistical significance to explain the variation amongst judge’s rates. My results show that judges in republican voting states have denial rates 30 percentage points higher than their counterparts and male judges have denial rates that are 8 points higher than female judges.

## <p align="center"> INTRODUCTION
There are over 650 immigration judges presiding across 68 immigration courts. Appointed by the Attorney General of The United States, these judges rule on cases regarding asylum seekers. There is no surprise that denial rates vary from judge to judge across the country, but the variation between judges in the same immigration court also varies dramatically. For example, Judge Paul McCloskey had a denial rate of 91.3% while the Honorable Lawrence Burman had a denial rate of only 15.3% and they are both currently assigned to the Arlington Immigration Court. This continued to puzzle me since asylum cases are randomly assigned to a judge’s docket which is supposed to help normalize distribution of cases. This issue of variation amongst judges is not new because Karen Musalo, director of the Center for Gender & Refugee Studies at the University of California Hastings School of the Law in San Franciso said in an interview with Reuters that “It is clearly troubling when you have these kinds of gross disparities,” (Rosenberg, 2017). Whether or not I believe her statements to be true, I still believe the topic is worth investigating.

## <p align="center"> LITERATURE REVIEW
Many organizations have studied the variation of asylum decisions, but none have more insightful information than Transactional Records Access Clearing house (TRAC) at Syracuse University. TRAC constantly produces studies and analyses on a variety of topics, but a study from 2018 titled Asylum Outcome Continues to Depend on the Judge Assigned had practical significance. The report analyzes the variance of rates by different classification such as the specific courts and similarities, but notes “that while judge-to-judge decision disparities have long existed, between 2010 and 2016 judge-to-judge decision disparities got worse.” (TRAC,2018). To me, this signifies that it is an ongoing scenario that deserves to be studied. Tracs results were as follows, “Under these circumstances any large differences in the denial rates of individual judges are unlikely to be the result of differences in the nature of the incoming cases. Instead, they are likely to reflect the personal perspective that each judge brings to the bench.” (TRAC,2018).

&nbsp;
The United States Government Accountability Office (GAO) also does a very thorough report into variation amongst immigration courts and judges. A report from 2008 titled Significant Variation Existed in Asylum Outcomes across Immigration Courts and Judges deeply into factors that could explain the extreme variation. They used probability parameters to try and predict the likelihood of judge’s decisions. GAO was able to access more personal data on the judges and were able to include variables like race and age. Their study produced the following results: “the immigration judge characteristics that had significant effects on asylum decisions, at least when we considered each characteristic one at a time, were gender, length of service as an immigration judge, veterans preference, prior public immigration experience, and prior experience doing immigration work for a non-profit organization.” (GAO,2019). These variables were a basis for my research and guided me towards my results.
## <p align="center"> MODEL STRUCTURE
This study utilized an OLS model that would attempt to explain the variance in denial rates using descriptive variables. The model uses regression analysis to describe the strength of relationship between denial rates and descriptive traits of judges (e.g., sex, salary, democrat) that would help identify trends. It has been stated many times that judicial philosophy and identity influence asylum decisions, therefore I tried to replicate judicial philosophy with my variables. A judge’s philosophy could be crafted in law school or given to him by an appointing superior. My regression model, variables, and definitions are listed below.

<p align="center"><img src=https://github.com/CTorresKnox/Technical-Portfolio/assets/144376690/62a47742-6988-41bc-aa9c-c50d0fdd8ee7>
<p align="center"><img src=https://github.com/CTorresKnox/Technical-Portfolio/assets/144376690/0702c30b-5df3-4bf1-969e-c999cc4f3000>

&nbsp;
My project does not look at the entire population of immigration judges, over 650, but rather focused on a cross sectional sample of 100 randomly selected judges which I will discuss shortly. It is worth mentioning that the “year appointed” also identifies the appointing Attorney General, which allows me to group judges by who appointed them, indicating an appointing political party. My hypothesis is that certain characteristics will be able to explain the erratic denial rates. I hope to Identify certain traits that can be used to predict denial rates amongst judges in the future. The alternative hypothesis is that no traits can explain the denial rates; however, even if we reject the null, we can still identify characteristics that increase denial rates.

## <p align="center"> DATA STRUCTURE
The data for this study with originally sourced from the Transactional Records Access Clearing house (TRAC) at Syracuse University. Their sources provided me with judge specific information including denial rates, year appointed, and educational and professional summaries. Building off this data, I generated multiple variables from government sources like The Executive Office for Immigration Review (EOIR), The U.S Department of Justice (DOJ), and The United States Citizenship and Immigration Services (USCIS). Ancillary websites such as specific government offices were very helpful in finding data. Descriptive statistics of each variable are shown below.

 <p align="center"><img src=https://github.com/CTorresKnox/Technical-Portfolio/assets/144376690/e54c4ca5-2357-423c-9bcf-246b024a10f3>

&nbsp;
The parameters for this data include a “snapshot” of asylum decisions by judge from 2017 -2022. Each denial rate is an aggregated average from the 6 years selected. I randomly selected 100 judges across all immigration offices and assigned them a random identifier. Once the data was completed, I had a panel data set with 100 individuals and over 10 independent variables to help explain denial rates.

## <p align="center"> RESULTS & ANALYSIS
My results produced insightful results, and yet we still must reject our null hypothesis in favor of the alternative. All variables were preforming as expected except the private schooling variable. The estimate relationship was thought to be negative under the assumption that private schooling would cultivate a more lenient and liberal personal philosophy. The model can only explain roughly 40% of the variation in denial rates amongst judges which is depicted in the R-squared statistic. However, since judicial denial rates differ so extremely, describing 40% of that variation with only four independent variables could be considered a success to some.

<p align="center"><img src=https://github.com/CTorresKnox/Technical-Portfolio/assets/144376690/c6da4eb6-d4fc-47ab-9fef-41a97cc2ef25>

&nbsp;
My model relays the following information, Judges in republican voting states have denial rates that are 29.87 percentage points higher than their counter parts. The main results also illustrate that male judges have denial rates that are approximately 7.7 percentage points. Privately educated judges have denials rates just a
little bit higher than publicly educated judges at 5.5 percentage points. The appointment year variable demonstrates a .47 percentage points variance in denial rates between different appointment years.

<p align="center"><img src=https://github.com/CTorresKnox/Technical-Portfolio/assets/144376690/6ae1683f-ab05-4a9a-bb1c-55cff885cca5>

&nbsp;
Not all my variables ended up being main driving traits due to high standard deviations and a lack of correlation. I assumed that the year a judge was appointed might have more significance since judges are appointed in groups by the Attorney General. My results show that the year appointed variable had the smallest standard deviation, but this is irrelevant due to the data being in years, and there are no means or averages for years. The republican state variable had one of the highest standard deviations, but I believe this is true because the difference of denial rates within each state are still quite large. The constant is also negative with a negative t-statistic which implies that the relationship
is negative and would show a downward trend when plotted or graphed.

## <p align="center"> SUMMARY & CONCLUSION
The model that was used for this research could not accurately explain the relationship between denial rates and specific characteristics of Judges. This requires me to deem the model not statistically significant, and to reject the null in favor of the alternative. Although the model was statistically unfruitful, I was still able to identify 3 drivers or influential variables, that increase a judges denial rate. Those traits are if a judge being male, whether the judge works in a republican state, and if they attended a private law school. These traits could be useful in understanding why asylum denial rates vary so much among immigration court judges.

&nbsp;
I recommend a follow-up study be done to further analyze this situation. In future study I will have more in depth data that can describe individual judges better. I would also narrow the focus down to immigration judges in the same court rather than across the country. This step is essential in making sure that the judges being studied are receiving the same types of cases at random. A full analysis of all judges would also increase the accuracy of the data rather than a sample of 100, but that increases the overhead tenfold. I recommend using my results from this study as a base to build an even more in depth and accurate model. 


## <p align="center"> WORKS CITED
“Asylum Decisions and Denials Jump in 2018.” TRAC Immigration, Transactional Records Access Clearinghouse, 29 Nov. 2018, trac.syr.edu/immigration/reports/539/ 

&nbsp;
“Asylum Outcome Continues to Depend on the Judge Assigned.” TRAC Immigration, Transactional Records Access Clearinghouse, 20 Nov. 2017, trac.syr.edu/immigration/reports/490/ 

&nbsp;
“Asylum Process in Immigration Courts and Selected Trends - CRS Reports.” CRS Reports, Congressional Research Service, 15 May 2023, crsreports.congress.gov/product/pdf/R/R47504 

&nbsp;
“The Civil Employee’s Resource.” FederalPay.Org, FederalPay, federalpay.org/. Accessed 2 Dec. 2023.

&nbsp;
“GAO-08-940 U.S. Asylum System: Significant Variation Existed in Asylum ...” GAO, United States Goverment Accountability Office, Sept. 2008, www.gao.gov/assets/gao-08-940.pdf   

&nbsp;
“Judge-by-Judge Asylum Decisions in Immigration Courts FY 2017-2022.” TRAC Immigration, Transactional Records Access Clearinghouse, 26 Oct. 2022, trac.syr.edu/immigration/reports/judge2022/  

&nbsp;
Rosenberg, Mica, et al. “For U.S. Asylum Seekers, Some Judges Are a Better Bet than Others - Reuters.” Reuters Investigates, Reuters, 17 Oct. 2017, www.reuters.com/investigates/special-report/usa-immigration-asylum/   

&nbsp;
“Workload and Adjudication Statistics.” Executive Office for Immigration Review, The United States Department of Justice, 10 Oct. 2023, www.justice.gov/eoir/workload-and-adjudication-statistics 
