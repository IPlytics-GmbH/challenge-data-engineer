# IPlytics Data Engineer challenge
This challenge is for candidates for the position "Data Engineer".

## Overview
Our platform lets users search for Patents, Standards and Declarations, amongst other things. Before data is available on the platform in a clean and structured way it has to go into a defined data model.

We want to know how well you can do the following:
* Creating a well-structured data model out of some flat CSV files
* Implementing a simple application to load data into the database structure you have created
* Performing analysis on the data once it's been loaded

## What we provide you
Fork this repo or clone it to your local environment.

Within this repo you will find three csv files in the folder `/dumps`. Each of these files contain data for different document types which should be linked together.

### Patents
A patent is a form of intellectual property that gives its owner the legal right to exclude others from making, using, selling and importing an invention for a limited period of years, in exchange for publishing an enabling public disclosure of the invention.

A patent is published at some point by a patent office and contains information about the inventor and the applicant (usually a company). Beside that it also has a legal status information (e.g. granted or lapsed). Due to prior art search a patent has to cite other patents which have covered fundamentals for the new invention. Patents usually are published as a group of patents (called a patent family defined by [INPADOC](https://worldwide.espacenet.com/help?locale=en_EP&method=handleHelpTopic&topic=legalstatusqh)) in order to cover multiple patent offices.

### Standard
Standards are requirements, specifications, guidelines or characteristics that can be used consistently to ensure that materials, products, processes and services are fit for their purpose. In the domain of telecommunication, they are often jointly developed by the stakeholders (e.g., Samsung, Apple, Huawei, Ericsson, etc) and state entities. When a consensus is reached, the standard is published by a Standard Setting Organization. The extent of relevance of a standard is often quite narrow, that's why standards often refer to standard projects, which make comprehensive specifications. As needs evolve, a standard is often adjusted and there is a version history to follow those evolutions.

### Declarations
Companies or organisations work with a standard-setting organisation (like ISO or ETSI) to "declare" their patent to be a necessary part of a standard. So there is a relational connection between patents and standards, which we can model as a "declaration".

## What we want you to do

You must solve a few small challenges in order to pass our test. In addition to doing the tasks below, we want to see that you can:

* Present your solution in a clear and readable way, with good documentation
* Write clean code and don't overcomplicate it
* Be creative in your analysis!

Here are your tasks:

### 1. Create and present the data model
You can use any tool of your choice for this, for example [draw.io](https://app.diagrams.net/)

What you should aim for:

1. Stable identifiers for entities and documents
1. Reduced data redundancy
1. Clear and well-defined relations between entities

### 2. Write DDL to create a SQL database
Transform your designed model into executable SQL statements which can create a database schema. MySQL compatible is preferable.

### 3. Application for loading data into MySQL database
Write a small application to load data from the provided CSV files into your database. Java or Python are preferred. There is no need to write code from scratch to do simple work. We want to see your use of a framework such as [Spring Batch](https://spring.io/projects/spring-batch) which minimises redundancy.

### 4. Data analysis
Now that you have loaded all this data, which indicators or metrics could you calculate from it? We would like to see some samples of creative SQL queries or other calculations we could run on the data, to extract interesting data points, or calculate values. 

## How to submit
Once you're happy with your work and want to submit, `zip` your work and submit it via email to our HR manager. If you have used git to track your changes, remember to include the whole assignment directory (including hidden files), so we can see your git commit history.

Best of luck and thanks for taking the time to complete this challenge.
