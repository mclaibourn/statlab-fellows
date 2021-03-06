## 2018-10-31

* Consultations:
    * Curry faculty; more work on her nutrition study.
    * Stat/Econ undergrad; walk-in. Help reshaping data in R. Very challenging consult that resulted in discovering the separate_rows function in tidyr. 
    * Sociology PhD student; more help with data wrangling in Stata, also some help implementing and visualizing mixed-effect models 
    * Nursing PhD student; help debugging an R function she wrote to download files from noaa.gov
    * A little more stats help for my Rwandan client. 

* Research/Learning:
    * Spent considerable time looking into using the boxr and here packages for the presidency project.
    * Completed Scalable Data Processing with R DataCamp course
    * Working through _Discrete Data Analysis with R_ book. (Reported an error to the author)
    * Started work on a StatLab blog post that explains how to assess Type S (sign) and Type M (magnitude) errors as outlined in Gelman and Carlin’s 2014 paper. I think it’s an interesting supplement to traditional power analysis. The paper is accessible, but I wanted to write a blog post that fills in gaps in the paper where the authors assume certain statistical concepts. 


## 2018-10-24

* Consultations:
    * PhD candidate at Darden. Had concerns about data not being normally distributed for a t-test. Pointed him to a journal article that explicitly addressed his concern. It showed through simulations that the Normality assumption was sufficient but not necessary for the validity of the t-test. https://www.annualreviews.org/doi/pdf/10.1146/annurev.publhealth.23.100901.140546 
    * Visiting Scholar, Architecture; help with interpreting coefficients in a model with log-transformed response variable. Referred her to my blog post, https://data.library.virginia.edu/interpreting-log-transformations-in-a-linear-model/ Also provided help getting started with linear mixed-effect models
    * PhD student, Sociology; help reshaping data in Stata
    * Psych faculty; help with polishing barplot in base R graphics; also how to accomplish same plot with ggplot2 and jtools packages. 
    * PhD student, chemistry; Help getting started with logistic regression and effects plots in R
    * Curry faculty; more work on nutrition study, including data cleaning and some exploratory work.

* Research/Learning:
    * Bayesian Data Analysis workshop
    * Back up Text Analysis part 1 workshop
    * Read a good article by Gelman, Ethics in statistical practice and communication Five recommendations http://www.stat.columbia.edu/~gelman/research/published/SIGN_15(5)_09_InPractice_Gelman_EthicsAndComm.pdf   
    * Started working through _Discrete Data Analysis with R_ book
    * Working through DataCamp course, Scalable Data Processing in R


## 2018-10-17

* Consultations:
    * Kinesiology Faculty; once again helping out with a study that requires a bit more work than usual. There’s potential to be a co-author. We’ll see. Grant-funded work. Spent most of the day Monday cleaning and exploring the data. 
    * Engineering grad student; some help with using and interpreting model selection criteria.
    * Nursing PhD candidate (drop in). Help with running multiple imputation on subsets of her data.
    * Architecture, Visiting Scholar (drop-in); help with running many regressions on subsets of her data; showed her how to use lapply           
    * Ph.D. Student, Civil Engineering (drop-in); help with reading Qualtrics CSV files into R and some various debugging of R code chunks.
    * Curry PhD candidate; some help and advice with interpreting results of a factor analysis and pairwise comparison of means after ANOVA.

* Research/Learning:
    * Back up Michele's Text Analysis Part 1 workshop
    * Review/Revise Bayesian data analysis workshop (teach on 2018-10-18)


## 2018-10-09
* Consultations: 
    * PhD candidate, Curry (2x). Help implementing and interpreting random-intercept model in SPSS. Did this using Zoom, which I must say was very easy. Much more pleasant than using Skype. Consulted again over email regarding some follow-up questions about evaluating model assumptions
    * PhD candidate Anthropology; conducted archaeological survey and excavations on a sugar plantation. Needs to analyze the artifact data she collected and wanted some guidance with the statistics. Talked about some different approaches as well as using ggplot to help create some basic visualizations. Sent her an R script to help her plot some means with error bars
    * Psych faculty. Help iron out some issues with creating plots to demonstrate kurtosis. Also help modify an R function for calculating power to have a more descriptive title.
    * Nursing PhD candidate. Questions about identifying and dealing with missing data. This is air quality data. I think she wants to impute missing data from certain stations with available data from nearby stations. I think. I’m still trying to figure out what exactly she wants. We’ve been doing this over email. Sent her some sample R code to help her get started exploring the missingness in her data.

* Research/Learning:
    * teach ggplot2 workshop (2018-10-03)
    * Review/Revise Bayesian data analysis workshop (teach on 2018-10-18)
    * Wrote up instructions for getting started with `boxr` package for working directly with files on box.com: https://github.com/uvastatlab/statlab-fellows/blob/master/resources/using_boxr.md
    * working through data camp course: Bayesian Regression Modeling with rstanarm
    
* Admin:
    * out of office Thurs, Oct 11 - Mon, Oct 15


## 2018-10-02
* Consultations: 
    * Politics PhD candidate; Looking for advice getting started with text mining Chinese social media and identifying types of propaganda. Suggested she start with a small collection of text and start working on getting it into R/Python, creating a corpus, creating a TDM, summarizing features of the text, etc to see if she can do what she wants to do. 
    * Biology grad student; asked about non-parametric 2 way anova. I couldn’t find anything other than a Friedman test, which I don’t think is what he needs. Mentioned that the usual parametric ANOVA is fairly robust to departures from normality and may be fine. Provided some simulations that showed non-normal and heteroscedastic data can be virtually indistinguishable from Normal data from a graphical standpoint (and suitable for ANOVA) but still be rejected by shapiro and levene tests. The point being we should use some judgment before dismissing data as non-normal or having non-constant variability based solely on a hypothesis test. Simulation code here: https://gist.github.com/clayford/dee4efbe5dd9103751a3565a94b164f7
    * Psych faculty; needed some programming assistance in R. Wanted to automate an R script so it could be run on various data sets and collect the output and plots.
    * English undergrad; referred to me by Scholars’ Lab. Writing a thesis that explains PCA and asked if I could review for accuracy.
    * Darden PhD candidate; help reshaping wide data to long. Also help getting started with mixed-effect models.
    * visiting scholar, Biology; help clean and reshape data and create bar plots of counts and proportions

* Research/Learning: 
    * Review/Revise ggplot workshop (teach on 2018-10-03)
    * Review/Revise Bayesian data analysis workshop (teach on 2018-10-18)
    * Investigate how to use `boxr` and `here` packages in R, potenitally for use with public presidency files
    * Investigate running obust linear regression with bootstrapped standard errors: https://gist.github.com/clayford/8912972554b8b44b0ff12d69660338c0

## 2018-09-25
* Consultations: 
    * Master of Science Student, Systems and Information Engineering; help with statistical analysis of experimental data. Had run 10 t-tests after an ANOVA. Suggested using adjusted p-values via Tukey’s pairwise comparisons. Also review how to check ANOVA assumptions.
    * undergraduate; help installing VMware client for the Hive, and then getting started with Stata on the hive.
    * EnviSci faculty; has dataset of atmospheric concentrations of numerous gases taken over time and space. Interested in analyzing the different contributions from different emission sources to the total concentrations. For example 50% of the methane concentration is attributed to oil/gas and 50% to rice cultivation. Very challenging consultation, especially since she doesn’t have any training data where she knows the proportion of contributions. 
    * Curry PhD candidate; seeking advice regarding how to handle missing data for mixed-effect modeling
    * UVa staff; provided some assistance with estimating power of a randomized complete block design for a given number of blocks.

* Research/Learning: 
    * Data Wrangling with R, part 2 and part 3 workshops
    * Review/Revise ggplot workshop

* Admin:
    * Town Hall meeting
    * R users meetup


## 2018-09-19
* Consultations: 
    * Commerce faculty; meeting to review and revise off-grounds housing web-scraping script to make it more robust to various departures from expected text. Made significant revisions to script.
    * Nursing PhD candidate; help merging date and time columns and formatting as date-time class. 
    * Staff, Emergency Medicine Research Office (EMRO); Trying to use the document-term matrix for association/cluster analysis. Suggested looking into topic-modeling at first but then realized cluster analysis might be better for what he wanted. Pointed to him some resources to help get him started. 
    * Grad student, Civil Engineering; Research involves using two types of neural networks to forecast groundwater level. Wanted to select better model. Suggested that instead of a t-test of the RMSEs between the two models that he take the difference in the 1000 RMSEs from the two models and analyze the distribution of differences with percentile/BCa intervals.
    * Undergrad, A&S; Needed some help understanding Excel instructions in a class assignment. Confused about how to use Excel to take a random sample from a sample frame.
* Research/Learning: 
    * final preparations for DWR part 3 workshop
    * Getting familiar with ggplot2 version 3 and seeing if there's anything of note to incorporate into my upcoming workshop
* StatLab article ideas (just some ideas off the top of my head! No guarantees!):
    * A primer/intro on using Stata's margin commands (possibly a series of articles)
    * A primer/intro on replicating the results of Stata's margin commands in R (possibly a series of articles)
    * Getting started with rate models
    * Getting started with CFA
    * Boostrapping basics with examples
    * Tips and strategies for simulating data in R


## 2018-09-10
* Admin:
    * Backed up Intro to R workshop. Always interesting to see what confuses new R users. This time someone was confusing objects in her global environment with files in her working directory. Totally understandable if you think about it.
* Consultations:
    * McIntire faculty; asked for help scraping housing information from the UVa off-Grounds Housing Service web site. Wrote an R script to do this: https://gist.github.com/clayford/3ddaca6b4d4f3d2daf8d9a49c8fbc5a2
* Research/Learning:
    * Getting ready for 3 part data wrangling with R workshop series.


## 2018-08-31
* Admin: fork statlab-fellows and sync public presidency repos; work with MPC to establish GitHub flow
* Consultations: 
    * Darden PhD candidate; help selecting, implementing and interpreting statistical analyses for his dissertation. 
    * Econ PhD; had some survey data she collected and noticed that a particular response seemed to depend on who asked the question. Suggested she run a mixed-effect model to control for the variation between survey administrators.
    * surgery resident; has data on vascular surgeries, wants to investigate whether or not certain medications are helpful post-surgery. Data is in Excel, has imported to Stata, wants help cleaning data in Stata. Data is restricted and requires access to a server. He could not access server or even get on Internet while in Brown. (I’ve noticed this a lot with medical employees.) Referred him to Data@HSL.
* Research/Learning:
    * non-linear regression
    * neural networks
    * simulating data from binary logistic model
    * Gelman, Honesty and Transparency are not enough: http://www.stat.columbia.edu/~gelman/research/published/ChanceEthics14.pdf
    * Gelman blog post, Some clues that this study has big big problems:
https://andrewgelman.com/2018/08/29/some-clues-that-this-study-had-big-big-problems/

