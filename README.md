# Foresight BI E-learning Weekly Enrollment Report
![](intro.jpg)
## Introduction
This is a Power BI project on the e-learning dataset provided by Foresight BI & Analytics which is a consulting and training firm that specializes in developing Microsoft Power BI reporting solutions and training for individuals and organizations. The goal of the project is to help management make informed decisions on improving student engagement on the platform and the course curriculums.
## Problem Statement
Management wants to understand the weekly performance of the e-learning platform. Among what management wants to determine are:
- Number of new users on the platform compared to the previous week.
- Percentage of new users that enrolled in courses compared to the previous week.
- Active students on the platform compared to the previous week.
- Number of students who completed a course this week compared to the previous week.
## Skills demonstarted
The following Power BI skills were incorporated into this project:
- Data transformation using Power Query Editor.
- Data modelling on Power BI.
- Knowledge of DAX functions. ADDCOLUMNS, CALENDARAUTO, YEAR, MONTH, FORMAT, WEEKNUM, DATE, CALCULATE, DIVIDE, COUNT, VAR, RETURN,  IF, and USERELATIONSHIP functions were used in this project.
- Data visualization on Power BI.
## Data sourcing
The dataset is a (anonymized) real-life dataset provided by Ahmed Oyelowo (MVP, MCSA, MCT, AFM) of Foresight BI & Analytics. Here's the link to the [dataset](https://docs.google.com/spreadsheets/d/1M3INoxFT5tzmjaDOS68TG4xfx7x4LERd/edit?usp=sharing&ouid=109205170271109304266&rtpof=true&sd=true).
## Data transformation
For the analysis, only the Courses, Enrollments, and Users sheet were transformed with Power Query Editor, the datetime columns in the sheets were transformed to date only columns for a clearer and precise analysis. There were no duplicates in the dataset.
## Data modelling
The model uses a star schema with multiple inactive relationships between date columns in the dataset. There are two (2) fact tables and one (1) dimension table. The Courses table (dimension) is joined to the Enrollments table (fact) via a one-to-many relationship. The Users table (fact) is also joined to the Enrollments table via a one-to-many relationship. A separate calendar table (dimension) was created to aid the analysis and since there can be only one active primary key relationship between two tables at a time, it was important to also create inactive relationships to answer the business questions.
![](model.png)
## Analysis and Visualizations
