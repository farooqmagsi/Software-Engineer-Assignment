
Title And Authors:-

An Empirical Study on the Impact of DE implicitization on Comprehension in Programs Using Application Frameworks.

•	Jurgen Cito From USA

•	Jiasi Shen   From USA

•	Martin Rinard From USA

•	Conference Program icse-2020

Introduction And Motivation:-

Ruby on Rails introduce abstractions with the goal of simplifying development for particular application domains “example web development”. Promoter Of these frameworks argue that the high learning curve introduced by the abstractions are justified because they result in increased productivity for expert developers. Continuing the example of Ruby on Rails,
•	Implicit flow of dynamic languages and dynamic dispatch.
•	Magic functionality introduced through metaprogramming.
•	Behavior in the codebase without explicit flows due to abstractions in application frameworks.
However, a downside is that programs using these frameworks may perform low-level actions not apparent in the source code, which often appear as unpredictable behavior or unexpected semantics 1, 2, 7–9 to non-experts. However, an unfortunate ancillary consequence is that programs written in these frameworks are often hard to understand for non-experts and newcomers to the codebase.


Research Methodology:-

Research Questions,
Question No,1:- Do deimplicitized programs reduce the time needed to complete comprehension tasks on the corresponding implicit programs?
Answer:- There is no difference in the response time between participants that access or do not access the depoliticized programs.: The response time is shorter for participants that access deimplicitized programs than participants that do not.
Question No,2:- Do deimplicitized programs increase the correctness of comprehension tasks on the corresponding implicit programs?
Answer:- There is no difference in the correctness of responses between participants that access or do not access the deimplicitized programs. The correctness of responses is higher for participants that access deimplicitized programs than participants that do not.
Question No,3:- Does the participants’ expertise in the application frameworks influence the time to complete or the correctness of the tasks?
Answer:- In this Experiment we will conduct two separate experiment
Experiment I focuses on novices. 
Experiment II focuses on experts
For each experiment we will independently test the two hypotheses described above.
Materials And Objects:- Part of our study objects we use open source applications of various sizes and complexities that are built with application frameworks. Specifically we use the Ruby on Rails projects in the experiments.

•	Enki, Content Management.

•	Fulcrum, Agile Project Management.

•	Kandan, Online Chat.           

•	Blog, Sample Application.  

Each of these applications consist of a user interface as a web page and a back-end server that accepts API calls from the web browser. When an API is called, the application server translates the input parameters into SQL queries against a relational database and returns results extracted from the results of the queries. The goal is to allow the deimplicitized code to provide similar information as in potential deployment scenarios.

PARTICIPANTS And SUBJECTS:-

We recruit participants with software development experience who have at least one year of Python programming experience and are familiar with relational databases and SQL syntax. 

EXECUTION  PLAN:-

We assign participants into two groups,
Control Group participants are shown only the implicit programs.
Treatment Group participants are shown both the implicit programs and their corresponding deimplicitized programs.
To familiarize participants with the study environment, we plan to start the session with a warm up task to explain the setting. Participants are then asked to comprehend several application APIs. For each API, participants answer questions about the functionality shown in the code. As soon as the code and question are displayed, we automatically start to measure the time to task completion, which is completed as soon as participants move on to the next question or complete the experiment session.

Result:-

The Result of this Study And Research is that, We plan to present summary statistics mean, median, standard deviation, max, min over the treatment groups and overall for the dependent variables time in seconds, number of correctly fulfilled tasks. As for significance tests, we plan to follow a frequentist approach. We would first test for normality by conducting a Shapiro-Wilk test. Depending on the distribution, we would then either perform a ttest or Mann-Whitney U test. We will do this for our variables Time Spent and Correctness We initially calculated effect size as part of our power analysis. We also set out to estimate the extent of how substantially different the measures in our full dataset are by calculating the effect size again. We choose the particular procedure to calculate effect size given the distribution of our sample measures.

