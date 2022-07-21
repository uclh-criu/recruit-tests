# Software Developer Technical Test

## Objective

This exercise is aimed at evaluating the applicant’s skills in understanding and solving a scenario that can be
presented as part of this role. The exercise focuses on key technologies and abilities required from the applicant,
with restrictions given by the environment in which the successful post-holder will interact, but also leaves room for
the applicant to highlight their skillset in the areas they are most comfortable with.

The final product will demonstrate the applicant’s ability in handling a given dataset, applying data management tools,
and producing a webservice to access the information, with the option of proposing a persistence back-end and user
interface.


## Evaluation

The outcome produced by the applicant will be evaluated by a multidisciplinary team of experts, including their future
line manager, with a focus on the following:

 - Code review: code quality, structure, readability, maintenance.
 - Functionality: required and optional, completeness, correctness.
 - Documentation: available information to guide other developers and or users
   on how to access the system, comments, readme.
 - Deployment: simplicity or complexity to execute the solution, dependencies,
   deployment process.


## Background

A team of scientists from an external university is preparing a national research study to analyse the distribution of
hospital admissions and outcomes by age, sex, and ethnicity. Before moving to a step where they will require extensive
patient datasets from several hospitals, including UCLH, they decide to execute a Feasibility Study consisting in the
collection and analysis of a small subset of indicators. With that information, the researchers expect to have a better
idea of whether UCLH would be a suitable site for their future studies.

The Information Governance team at UCLH approves the feasibility project under the condition it **does not access 
identifiable** patient information.

In consequence, the researchers ask UCLH to **provide the following data points**:

 - Fake Patient ID: to track persons across admissions
 - Year of Birth: to determine age groups
 - Year of Death: if applicable
 - Sex at Birth
 - Ethnicity
 - Admission details: Date and Time, Source and Outcome


## Requirements

As agreed within the team, the best approach in this scenario is to provide an online tool for the researchers to 
query the data.

The Data Manager has extracted two initial CSVs with a small set of **identifiable** Patient and Admission information.


### Essential features

You are required to implement a **webservice** that serves the information found in the CSVs in an appropriate 
format.
_While the team focuses on Spring and Python, you can use the programming language and libraries of your choice._

You are also asked to **share the code** via a platform that can be accessible by the rest of your team (GitHub, 
GitLab, or similar).


### Optional features

Additional to the core requirements, you are invited to implement optional features to enhance the platform.
_These modules are not mandatory but will allow you to demonstrate your abilities in different areas, and help the team
identify your strengths._

 1. The CSVs provided are currently small, but you know the following extractions can contain millions of rows. With 
    this in mind, you decide to set up a **persistence layer with a database**, ingesting the data from the CSV files 
    and connecting it to your webservice API.

 2. Since the researchers will be overloaded with information from different hospitals and in different formats, you
    decide to implement a user-friendly **Web front-end** that simplifies querying the API and viewing results.

 3. Thinking you could support the researchers even further, you decide to implement – as part of the API or the
    front-end – features that analyse and **aggregate data** (e.g., number of admissions per sex).

 4. You work in a team and anyone could be moved onto this project, so you write and share **documentation** about how 
    to deploy, execute and use the tools. You also briefly explain, where applicable, your decisions on architecture,
    modelling and choice of technologies.

 5. The team uses Docker and Docker Compose to deploy heterogeneous and complex technology stacks in generic Linux
    servers. You decide it’s worth providing Docker files (“Dockerfile”, “docker-compose.yml”) to ease the deployment of
    your solution. _If you have never heard of or used it, this is a great opportunity to showcase your curiosity and 
    talents dealing with a new tool!_


## Things to keep in mind

 - **Quality** is better than Quantity. **Simple** is better than Complex.

 - Health-related data is highly sensitive and must be accessed/provided on a need-to-know basis. The CSVs provided
   contain fake data, but in the context of this exercise all names and dates of birth are considered Personal 
   Identifiers (PID) and should be protected from external access (year of birth alone, however, is safe).

 - The Optional Features are 100% optional, they exist to give us hints of the areas you feel most comfortable with. We
   are well aware that you might have commitments that make it hard to go deeper in this exercise. Whether you are 
   able to implement zero or more, you will have the opportunity to explain any choice during the interview.

 - If you feel uncomfortable with any technology that has been mentioned, do not worry, we are always learning! We value
   independence but we love teamwork. If you have general questions about the exercise (e.g., a requirement is not
   clear or you are stuck installing Docker), feel free to contact [uclh.criu@nhs.net](mailto:uclh.criu@nhs.net) 
   mentioning the
   job reference.
