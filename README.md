# **Course Title**<br/>by **Course Author**

README and sample lesson deadline: YYYY-MM-DD 

As part of the 'Course Spec' process, you will need to complete the following tasks:

- [ ] Edit this README by filling in the information for steps 1 - 7 according to our README rubric.
- [ ] Review [the documentation](https://instructor-support.datacamp.com/?q=spreadsheets) on creating Spreadsheets courses to create a capstone exercise for each chapter.
- [ ] Complete one sample lesson according to the sample lesson rubric.

## Course development resources

* Add video exercises: https://www.datacamp.com/teach/
* Add spreadsheet exercises: https://spreadsheets.datacamp.com/courses/ (Link to come)

## Step 1: Brainstorming 

This part of the 'Course Spec' process is designed to help guide you through course design by having you think through several key questions. Please make sure to delete the examples provided here for you.

### A. What problem(s) will students learn how to solve? (minimum of 5 problems)

- [ ] Write a list of ideas for problems that the students will encounter in the course.
> From a course on spreadsheets for finance:
>
>- How to design a Google Sheets interface to analyze the past performance of a stock 
>- How to display the past evolution of a stock price
>- How to compute stock returns
>- How to measure historical performance and risk
>- How to display the distribution of historical returns
>- How to model stock returns using the Gaussian assumption
>- How to use a benchmark to assess the risk and return of a stock


### B. What are the learning objectives of the course?

- [ ] Write a list of learning objectives for the course. These are not shown to the students, but they will be used to ensure your vision for the course aligns with the vision of your Curriculum Lead.

>Example from our scikit-learn course:
>
>- Learn the key concepts of supervised learning and how to implement them on real-world datasets;
>- Learn to distinguish regression from classification problems;
>- Learn to evaluate how well your classification and regression modes perform;
>- Learn best practices in supervised learning, such as splitting into test/train sets and k-fold cross validation;
>- Learn how to improve model performance by both preprocessing your data and regularizing your models.


### C. What functions will students use? Please be exhaustive.

- [ ] Write a list of ideas for the Spreadsheets functions that you want to use in the course. Please note that we packages, currently cannot support Google Sheets add-ons. If there are any important functions, methods, or commands that you want to teach, you can mention them here.

> Example from a course on spreadsheets for finance.

> Basic Google Sheets functions: SUM, PRODUCT, COUNT, IF, COUNTIF, AVERAGE, MIN, MAX, STDEV, PERCENTILES, ARRAYFORMULA,
> VLOOKUP, NORMDIST, NORMINV, CORREL.


### D. What terms or jargon will you define?

- [ ] Write a list of technical terms, jargon, and acronyms that will be used in the course and define them as well.

> Example from a course on pandas.
>
> - Tabular data: data with rows and columns
> - DataFrame: a pandas representation of tabular data
> - Merge: an opperation that combines two DataFrames based on common column values
> - Aggregate: a single value computed based on a set of values.  For example, an average applied to a column of numbers is an aggregate function

### E. What analogies or heuristics will you use?

- [ ] Write a list of analogies for concepts, heuristics for best practices, and any other non-technical explanations of things that may be helpful to students _(minimum of two)_.

>Example from a course on forecasting product demand. This analogy is likely intuitive to most people.
>
>Signal and noise - It's like trying to hear someone across a crowded room. Remove the noise, and you can easily understand what they are telling you.


### F. What mistakes or misconceptions do you expect? 

- [ ] Write a list of common mistakes _(minimum of two)_ that you think students will make. These can be programming mistakes, conceptual misunderstandings, or simply examples of things that are unintuitive. 

>Example from a course on generalized additive models:
>
>The difference between prediction intervals and confidence intervals.


### G. What datasets will you use? 

- [ ] Write a list of datasets that you will use in the course, a short description of each dataset (if it's not clear from the title), how you intend to use it and include a link to its source(s). You should aim to have between 1 and 8 datasets in your course.

- [ ] Upload these datasets to this repository.

Please avoid [overused datasets](https://authoring.datacamp.com/courses/design/brainstorming-datasets.html).

## Step 2: Who is this course for?

Terms like "beginner" and "expert" mean different things to different people, so we use personas to help instructors clarify a course's audience. When designing a specific course, instructors should explain how it will or won't help these people, and what extra skills or prerequisite knowledge they are assuming their students have above and beyond what's included in the persona.

- [ ] Please select the learner personas that align with your course. 
- [ ] Include an explanation describing your reasoning behind choosing the corresponding learner persona and any other relevant information.

Choose the appropriate learners for your course by following this link to [learner personas](https://instructor-support.datacamp.com/courses/course-design/learner-personas)

* Learner persona 1: explanation
* Learner persona 2: explanation
* Learner persona 3: explanation

## Step 3: Course outline

A typical course is structured as follows:

- Chapter 1 has three lessons. This chapter is shorter than the rest since it serves as an introduction to the topic.
- Chapter 2 has 3-4 lessons.
- Chapter 3 has 3-4 lessons.
- Chapter 4 has 3-4 lessons.

A typical lesson is comprised of:

- A video exercise with slides and script, e.g. [sample video exercise](https://spreadsheets.datacamp.com/courses/intermediate-spreadsheets-for-data-science/chapters/working-with-numbers/exercises/5).
- 2-4 exercises that review what is covered in the video exercise.

*Remind yourself about [course terminology](https://authoring.datacamp.com/courses/design#terminology-and-structure), then describe the flow of the course.*

> Example from a course on spreadsheets for finance

> Chapter 1 - Monitoring historical prices (the “Prices Panel”)
> In this first chapter, you’ll be introduced to the problem: you have a time series of monthly (historical) prices for the stock ABC from which you have to extract some meaningful information. You’ll be given some definitions (what is a stock? what are dividends?), and at the end of the chapter, you’ll be able to graphically represent the evolution of a stock price over a specific period.

>   * Lesson 1.1 - Historical prices and first metrics
>     * A learning objective: Identify relevant information of stock prices and dividends for a specific time period.
>     * Description: You’ll be introduced to the dataset. You’ll learn what is a stock, why its price changes over time, what are dividends and when a company decides to pay them out. Once the theoretical part is done, we’ll provide you with the first set of indicators to look at when dealing with a time series of historical prices for a stock: minimum, maximum and average price. At the end of the chapter, you’ll learn how to compute them using the functions MIN, MAX, and AVERAGE.
>     * Some functions introduced/used: COUNT, MIN, MAX, AVERAGE, COUNTIF, MINIF, MAXIF, AVERAGEIF
>   * Lesson 1.2 - Identifying dates with unusual prices
>     * A learning objective: Identify dates when extreme prices occurred using the LOOKUP function.
>     * Description: Once having obtained the extremes of the ABC price during the period under analysis, in order to have more and better insights, it is crucial to know when these extremes occur, at which dates. Then, you’ll learn how to use the VLOOKUP function.
>     * Some functions introduced/used: VLOOKUP
>   * Lesson 1.3 - Visualizing the price evolution
>     * A learning objective: Display the evolution of the price using standard plotting functions and include in the graph additional indicators such as minimum, maximum and average price.
>     * Description: We build the first interface. It’s time to put all together and show it in a meaningful chart. 
>     * Some functions introduced/used: Google Sheets plots

> Chapter 2 - Monitoring historical returns (the “Returns Panel”)
> In this chapter, the core of the analysis will switch from historical prices to historical returns. You’ll learn (and compute) the main performance indicators of past returns, both in terms of reward and risk. Finally, you’ll be introduced to risk-adjusted performance measures: indicators that take into account both reward and risk.

>   * Lesson 2.1 - From prices to returns
>     * A learning objective: Understand what is a financial return and compute returns from a time series of historical prices.
>     * Description: You’ll go through the concept of financial returns. What is a return? How is it computed?
>     * Some functions introduced/used: Simple division operator /, drag formulas, format with %
>   * Lesson 2.2 - Performance metrics
>     * A learning objective: Identify and compute both geometric, and arithmetic mean return using the functions AVERAGE, PRODUCT, ARRAYFORMULA, and GEOMEAN.
>     * Description: You’ll learn how to compute the effective rate of return of an investment, that is, the geometric mean return. Depending on the purpose of your analysis, you might also want to compute the arithmetic return, which is a simple indicator of the expected return you can get from that investment. Finally, there will be a brief explanation of the spreadsheet function that can be used to compute these metrics.
>     * Some functions introduced/used: AVERAGE, PRODUCT, ARRAYFORMULA, GEOMEAN
>   * Lesson 2.3 - Risk metrics
>     * A learning objective: Identify and compute key risk measures using functions such as STDEV and PERCENTILE.
>     * Description: You'll be introduced to the risk side of owning a stock. First, we’ll talk about the standard deviation, aka the volatility of the stock price over time. Maybe the most used risk indicator. Then, we’ll start having a look at the returns as a series of sorted values, and we’ll introduce the concept of percentiles, which can be used to define other popular risk-indicators (IQ ranges, historical VaR).
>     * Some functions introduced/used: STDEV (unbiased), PERCENTILE
>   * Lesson 2.4 - Risk-adjusted metrics
>     * A learning objective: Compute performance metrics that take risk into account.
>     * Description: In the final lesson of this chapter, you’ll be introduced to risk-adjusted indicators. Such indicators reveal how much risk was taken to achieve a return. In particular, we’ll focus on one of the most common risk-adjusted metric, the Sharpe Ratio.
>     * Some functions introduced/used: STDEV (unbiased), PERCENTILE

> Chapter 3 - Monitoring the distribution of returns (the “Distribution Panel”)
> In this chapter, you'll look at the full distribution of historical returns. First, you’ll learn how to build a histogram to describe the distribution of historical returns. Second, you’ll be introduced to the Gaussian distribution, a commonly used model for stock returns. You'll visually inspect if the Gaussian model is reasonable for the ABC stock returns. Finally, you'll understand potential flaws with the Gaussian model.

>   * Lesson 3.1 - Histogram of stock returns
>     * A learning objective: Create a histogram for the stock returns.
>     * Description: The learner will be driven step by step in the process of creating a histogram describing the distribution of past stock returns. After the graph has been generated, we’ll give the definitions of two indicators that describe the shape of a statistical distribution, that is, skewness and kurtosis.
>     * Some functions introduced/used: COUNTIF, (FREQUENCY + ARRAY FORMULA?), SKEW and KURT
>   * Lesson 3.2 - The Gaussian model
>     * A learning objective: Displaying the Gaussian distribution using the function NORMDIST.
>     * Description: You’ll be introduced to the Gaussian model. First, we’ll provide the theory behind, and then we’ll show some applications in spreadsheets and introduce some functions (NORMDIST,...). 
>     * Some functions introduced/used: NORMDIST
>   * Lesson 3.3 - Visual comparison of the distributions
>     * A learning objective: Superimpose the Gaussian curve on the histogram of stock returns in order to (visually) identify if returns fulfill the Gaussian assumption.
>     * Description: Start with the logic behind the process: the comparison of two distributions. This is possible by comparing the distribution of historical returns with a hypothetical Gaussian model in which the mean is the mean of average return, and the standard deviation is the standard deviation of the returns By looking how close (or how far) are one another, we can draw relevant information about the stock return distribution.
>     * Some functions introduced/used: NORMDIST
>   * Lesson 3.4 - Flaws in the Gaussian model
>     * A learning objective: Understand possible flaws/shortcomings related to the usage of the Gaussian model when modeling stock returns.
>     * Description: In this lesson, which will be mainly theoretical, we’ll make some considerations about the Gaussian model. We’ll discuss both the sides of the coin. First, we’ll explain why such a distribution is so popular; then, we’ll highlight what are the proven flaws that this distribution has when it is used to model stock returns.
>     * Some functions introduced/used: NORMINV

> Chapter 4 - Benchmarking performance (the “Benchmarking Panel”)
> In this final chapter, you’ll benchmark ABC stock against a market index and verify whether ABC outperformed the benchmark or not. The comparison process will be done through several steps/metrics. First, you’ll analyze the only cumulative returns. Next, you’ll extend the comparison using different indicators such as Sharpe Ratio and Drawdown. Finally, you’ll examine the linear relation between ABC stock and the benchmark through the correlation coefficient. At the end of the chapter, you’ll be introduced to more powerful and advanced spreadsheet features that introduce the interactivity feature in your analysis.
>   * Lesson 4.1 - Cumulative returns comparison
>     * A learning objective: Compare the performance of the ABC stock with a benchmark through a cumulative returns graph.
>     * Description: You’ll learn how to generate a cumulative return graph reporting the returns realized on both the ABC stock and the market index during the period under analysis.
>     * Some functions introduced/used: + and * operators.
>   * Lesson 4.2 - Performance metrics comparison
>     * A learning objective: Compare and rank different investments using indicators such as the Sharpe ratio and the Maximum Drawdown.
>     * Description: We’ll extend the comparison by using indicators (such as the Sharpe Ratio, the Sortino Ratio, and the Maximum Drawdown) that allow ranking different investments. 
>     * Some functions introduced/used: MAX, MIN, AVERAGE, STDEV (unbiased)
>   * Lesson 4.3 - Correlation analysis
>     * A learning objective: Assess the linear dependence between two securities through the Pearson Correlation coefficient. 
>     * Description: The learner will be introduced to the concept of historical correlation, an indicator which measures the linear dependence between two set of historical returns.
>     * Some functions introduced/used: CORREL
>   * Lesson 4.4 - Making it interactive!
>     * A learning objective: Make the application interactive to the user.
>     * Description: Maybe here just a video to show how to select a stock when several stocks are available. Same for the benchmark. Then we can extend to a particular time period.
>     * Some functions introduced/used: List selection, IF, VLOOKUP
  
  - [ ] Does each lesson have a clear learning objective?
  - [ ] Does each lesson include a brief list of functions or packages that the student will use?
  - [ ] Does the outline have at least 12 lessons and no more than 15?

## Step 4: Capstone exercises

Create a capstone exercise for **each chapter** of your course in the Spreadsheets authoring tool. **(Note: This is different from what you did when you submitted your course outline application, which was just one exercise for the entire course)** Let your Curriculum Lead know when you have completed this step so that they can review your exercises and provide you with feedback.

A capstone exercise should showcase how far learners are likely to get at the end of each chapter.

Please ensure that your capstone exercises meet our [Spreadsheet content guidelines](https://instructor-support.datacamp.com/courses/spreadsheets/spreadsheets-content-guidelines). Note that instructors DO NOT need to currently write SCTs for Spreadsheets courses as some changes are being made to the testing system.

## Step 5: Build ONE complete lesson on the Teach Editor and Spreadsheets authoring

This should include:
1. A video exercise with slides (this can be the same as or similar to slides/video that you already created for your audition).
2. Between 2 and 4 exercises that allow students to practice what you taught in the video exercise.  This does not (currently) include having instructors write Solution Correctness Tests (SCTs), but does include writing the success message for each exercise.

Why create a lesson as part of your course spec?

It will:

- Allow you to become familiar with the Teach Editor and Spreadsheets authoring tool along with our different exercise and slide types earlier.
- Give you a better understanding of course scope (e.g., what can be covered in a reasonable amount of time, and what must be saved for a future course - compared to creating just a course outline.)

In combination, this will result in faster course development time, a more frictionless course development experience, and prevent roadblocks that arise out of miscalibrated course scope.

Our experience working with over a hundred expert instructors over the past 4 years has taught us that the most challenging part of creating a DataCamp course is in understanding the scope of what can be covered in a lesson (and, by extension, a course). 

We believe that students learn best when their hands are on the keyboard, writing code, working with data, and solving problems. Consequently, our courses consist of short  3 to 4-minute videos separated by interactive coding exercises, with occasional multiple choice exercises interspersed. The videos are intended to teach students the concepts necessary to solve the exercises that follow. 

Four-minute videos correspond to between **400 and 600 words total** in the script. 

**Teaching data science concepts in this amount of time is not easy:** 
- It forces you to drill down to the essence of the concept and eliminate everything extraneous. 
- It requires a different approach compared to giving 50-minute college lectures.
- Writing such a script as part of your sample lesson will help you in creating a course outline that covers the right amount of content.

## Lesson Rubric and Process

### Process

**Timeline**

**Please work with your Curriculum Lead to ensure that all of the following boxes are checked.** Once that happens, the Content Development team will review the lesson within **3 working days**, and you must incorporate the feedback (if any!) within the next **3 working days.** 

**Feedback Delivery**

There will be no more than **2 rounds of feedback** by a Content Developer, and in each round of feedback, the Content Developer will be specific and unambiguous in explaining exactly what revisions are necessary before the course can be considered ready for handoff. If, after two rounds of feedback, the lesson is still not deemed acceptable by the Content Development team, DataCamp will not move forward with course development.

### Lesson Rubric

#### General

- [ ] Does the lesson consist of 1 video followed by 2-4 exercises?
- [ ] Are there at least 2 exercises?
- [ ] Is there no more than 1 multiple choice exercise?
- [ ] Is the script for the video between 400 and 600 words?
- [ ] Are the titles of the exercises and slides written in sentence case?
- [ ] Do the exercises run on our platform?

#### Video

- [ ] Are the slides dynamic? That is, is there movement on the slides, such as in the form of transitions between bullets or progression through a visual/schema?
- [ ] Are full sentences in slides avoided?
- [ ] Is there a clear learning objective and/or narrative that motivates why the concept is important?
- [ ] Is modeling of the Spreadsheets techniques covered in the exercises presented in the slides using visuals (relevant screenshots, GIFs, etc.)?
- [ ] Is the (trans)script written in complete sentences, without any bullet points or markdown? The script should correspond to exactly what you will say in the final recording and will be used to generate the subtitles for your course.

#### Exercises

- [ ] Context: 180-780 characters
- [ ] Instructions: 1-4 bulleted instructions
- [ ] Hints: 1-4 bulleted hints
- [ ] Success Message: Is there an informative success message?
- [ ] Submission Correctness Test: Is it implemented and does it respond if you enter the wrong answer?
- [ ] Are the instructions bulleted?
- [ ] Are the hints bulleted?

#### FAQs

##### Which lesson should I create for my sample lesson?

This is your choice. We recommend the final lesson of your course, as it has the following advantages:

- The concepts will likely be more advanced, and confirming that you can adequately teach the material in less than 600 words will verify that the course scope is appropriate.
- Similarly, the exercises will tend to be more advanced. Confirming that the exercises run on DataCamp and that the exercises meet our content guidelines will provide another check to verify that the course scope is indeed appropriate. 
- It provides clarity on where students will be at the end of the course and a clear stopping point that you can then work towards during the rest of course development.

**Whichever lesson you create, it is important to keep in mind the spirit of the sample lesson:** 
- it is an important check on course scope, 
- an opportunity to acquaint yourself with the tools you will be using to build your course, 
- and a chance to receive early feedback on teaching style to ensure you and DataCamp are aligned on course vision.

## Step 6: Revisit course outline

Having created your sample lesson, you should now have a much better understanding of course scope. This is an ideal time to revisit your outline and update it if necessary. Make sure that your lesson titles in your outline match up with the names of the video exercises.

## Step 7: Write course description and list course prerequisites

**Course Description**

Add a one-paragraph description of the course below. Please review these guidelines when creating it: https://instructor-support.datacamp.com/courses/course-design/datacamp-course-descriptions. 

> An example from a course analyzing survey data

> You've taken a survey (or 1000) before, right? Have you ever wondered
  what goes into designing a survey and how survey responses are turned into actionable
  insights? Of course you have! In Analyzing Survey Data in R, you will work with
  surveys from A to Z, starting with common survey design structures, such as clustering
  and stratification, and will continue through to visualizing and analyzing survey
  results. You will model survey data from the National Health and Nutrition Examination
  Survey using R's survey and tidyverse packages. Following the course, you will be
  able to successfully interpret survey results and finally find the answers to life's
  burning questions!

**Prerequisites**

*Which DataCamp courses cover topics that a student should be familiar with before attempting this course? Here are some examples:*

- [Spreadsheet Basics](https://www.datacamp.com/courses/spreadsheet-basics)
- [Data Analysis with Spreadsheets](https://www.datacamp.com/courses/data-analysis-with-spreadsheets)
- [Intermediate Spreadsheets for Data Science](https://www.datacamp.com/courses/intermediate-spreadsheets-for-data-science)
