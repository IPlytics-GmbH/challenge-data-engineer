# IPlytics data engineer challenge
This challenge is for candidates for the position "Data Engineer".

## Overview
Our platform lets users search for Patents, Standards and Declarations, amongst other things. Before data is available on the platform in a clean and structured way it has to go into a defined data model.

We want to know how well you can work with the following:
* Creating a data model out of flat structured csv files
* Turning data model into SQL statements
* Implementing basic application to load data into database

## What we provide you
Fork this repo or clone it to your local environment.

Within this repo you will find three csv files in the folder `dumps`. Each of this file contains data for different document types which should be interlinked together.

### Patent
A patent is a form of intellectual property that gives its owner the legal right to exclude others from making, using, selling and importing an invention for a limited period of years, in exchange for publishing an enabling public disclosure of the invention.

A patent is published at some point by a patent office and contains information about the inventor and the applicant (usually a company). Beside that it also has a legal status information (e.g. granted or lapsed). Due to prior art search a patent has to cite other patents which have covered fundamentals for the new invention. Patents usually are published as a group of patents (called a patent family defined by INPADOC) in order to cover multiple patent offices.

### Standard
Standards are developed with full consensus, that is, they are developed by experts with the aim of arriving at a common standpoint, taking the state of the art into consideration.

A standard is being developed and published by a standard setting organization and contains the involved authors. It also targets a main technology generation and refers to standard projects. A standard is constantly subject to changes therefore there is a version history.

### Declaration
One interesting aspect of industrial or technology standards is how they are composed. Companies or organisations typically work with a standard-setting organisation (like ISO or ETSI) to "declare" their patent to be a necessary part of a standard. So there is a relational connection between patents and standards, which we can model as a "declaration".


## What we want you to do

### Design and present the model graphically
You can use for this any tool (e.g. draw.io). 

What you should aim for:

1) Stable identifiers
2) Foreign keys
3) As less as possible redundant information
4) As much interconnected models as possible

### DDL to create a MySQL database
Please transform your designed model in executable SQL statements.

### Application for loading data into MySQL database
Please write an application (preferably in Java) to load the data into the database.

## How to submit
Once you're happy with your work and want to submit, `zip` the repo folder and submit it via email to our HR manager. Remember to include the whole assignment directory (including hidden files), so we can see your git commit history.

Best of luck and thanks for taking the time to complete this challenge.