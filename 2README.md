

Title And Authors:- 

Test Routes: A Manually Curated Method Level Dataset for Test-to-Code Traceability.

•	Andras Kicsi

•	Laszlo Vidacs

•	Tibor Gyimothy

•	Conference Program icse-2020

Introduction And Motivation:-

This paper introduces the Test Routes dataset and describes its properties and structure. The dataset includes method level traceability links for 220 test cases Software testing which aims to uncover the faults that lie within the software. In the case of a larger software system, staggering amounts of tests can be created as a byproduct of the development it is not rare for a system to incorporate tens of thousands of tests. Having a large number of tests, even telling which part of code a test aims to evaluate can mean a considerable difficulty. This problem, tracing tests to their units under test, is called test-tocode traceability. In many cases, it means more than just considering the methods a test case calls, which can be abundant. While good coding practices like following some kind of naming conventions can help this process, even these can not solve every problem. s. Compared to data used in related research, this dataset is a big step forward in granularity, in volume and in supplying the context to the tests.

Research Methodology:-

Traceability in software engineering research usually means the discovery of traceability links from requirements or related natural text documentations towards the source code. The dataset contains information on four open-source software systems written in the Java programming language. Joda-Time provides a replacement for the standard Java date and time classes which was widely used before Java SE 8. JFreeChart helps displaying various diagrams in several different formats in Java programs. Gson supports the serialization and deserialization of Java objects. JFreeChart is the largest of the systems but Joda-Time has the most tests, more than a third of its total methods are tests. The test cases are the methods aiming to assess a specific part of the software. e. They often contain one or more assertion statements and make method calls to conduct the evaluation. The test cases often enlist the aid of helper methods for setup or modularity purposes. These methods are customarily well separated from the production part of the source code. There can be multiple focal methods for a test case, or even none, for instance, if the test case evaluates a property of a whole class. These contextual calls and the calls made by the focal method can also be important.

Result:-

In this paper, we described a manually curated dataset, which contains traceability links for 220 test cases at method level granularity from 4 open-source Java programs. Test-to-code traceability provides the target of test cases in the production code. State-of-the-art algorithms are typically evaluated using a relatively small number of manually collected links. In addition, only very few of these links are available, which hampers the comparative evaluation of novel methods.. The dataset includes not only the traceability links but also highlights the context of the test and production methods. The whole dataset consists of more than 2000 categorizations of methods that were manually examined.
