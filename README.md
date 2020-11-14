# Descriptive-Analysis-of-Ride-Sharing-App-Prices- (Uber & Lyft)
---

> Author: Richard Taracha

> Date: 14/11/2020

![lyft and uber](https://user-images.githubusercontent.com/67068918/99152661-1f896980-26b4-11eb-832d-686bc14a1dce.jpg)

---

### Table of Contents
Sections headers used to reference locations of each destination:

- [External Data Source Validation](#external-data-source-validation)
- [Understanding The Context](#understanding-the-context)
- [Project Deliverable](#project-deliverable)
- [Recording the Experimental Design](#recording-the-experimental-design)
- [Summary Of Findings](#summary-of-findings)
- [Recommendations](#recommendations)
- [Author Information](#author-information)

---

## External Data Source Validation

According to https://www.nycgo.com/neighborhoods-boroughs/about-nyc-five-boroughs/, New York City has 5 main Boroughs namely: the Bronx, Brooklyn, Manhattan, Queens and Staten Island—each with dozens of neighborhoods lending their own local flavor

Our data set contains these boroughs confirmed using the formular df.Boro.Unique(): New Jersey', 'Manhattan', 'Bronx', 'Westchester', 'Brooklyn', 'Rockland County', 'Nassau County', 'Queens', 'Staten Island', 'Connecticut', 'All Boroughs' which is more than what the information above has indicated although the data contains the 5 main boroughs. The assumption is that the extra boroughs are within the 5 main boroughs.

The data is provided to the NYC open data by Department of Education (DOE) and can be accessed via https://data.cityofnewyork.us/Transportation/Bus-Breakdown-and-Delays/ez4e-fazm

> All personally identifying information has been removed from the data.

## Understanding The Context

With this project, I'm working as a Data Science Consultant and has been tasked to provide recommendations on how to reduce the cases of breakdown of buses in the city of New York. 

Given a dataset, I performed data exploration and data wrangling (data cleaning and analysis) then came up with some appropriate recommendations. 

#### Technologies and Tools

- Pandas
- Numpy

[Back To The Top](#New-York-City-Bus-Breakdowns---Data-Wrangling-with-Python)

---

## Project Deliverable
Deliverable is a python notebook that contains my solution:

* Notebook name: New York City Data Wrangling with Python.ipynb

Dataset Overview:
The dataset that was provided comes from the Bus Breakdown and Delay system which collects information from school bus vendors operating out in the field in real time. Bus staff that encounter delays during the route are instructed to radio the dispatcher at the bus vendor’s central office. The bus vendor staff are then instructed to log into the Bus Breakdown and Delay system to record the event and notify OPT. OPT customer service agents use this system to inform parents who call with questions regarding bus service. The Bus Breakdown and Delay system is publicly accessible and contains real time updates. All information in the system is entered by school bus vendor staff.

* Dataset name: hotel_bookings.csv
* Dataset Download Link: https://bit.ly/BusBreakdownDataset

[Back To The Top](#New-York-City-Bus-Breakdowns---Data-Wrangling-with-Python)

---

## Recording the Experimental Design
1. Define the Research Question
2. Data Importation
3. Data Exploration
4. Data Cleaning
5. Data Preparation
6. Data Analysis

Given the dataset, I performed data exploration, data wrangling (cleaning and analysis) in an effort to come with appropriate recommendations. 

As a start while performing data analysis, I derived the following questions from the given dataset: 
1. Which bus companies that had the highest breakdowns?
2. What were the top 3 reasons for bus delays?
3. How many students were in the buses when they broke down?
4. Which were most frequent reasons for bus breakdowns?
5. What were the most frequent reasons for the bus running late?
6. What was the average delay time of each reason type?


[Back To The Top](#New-York-City-Bus-Breakdowns---Data-Wrangling-with-Python)

---

## Summary Of Findings

- From my analysis, most of the delays were caused by late returns from field trips
- Heavy traffic and mechanical problems are the most frequent reasons for bus delays.
- G.V.C., LTD, LEESEL TRANSPORTATION CORP (B2192) and PIONEER TRANSPORTATION CO	are the bus companies with the highest number of breakdowns.
- There were a total number of 58329 students on the bus when it broke down and a total number of 890829 on the bus when it was running late.

[Back To The Top](#New-York-City-Bus-Breakdowns---Data-Wrangling-with-Python)

---

## Recommendations

From the above analysis, below are our recommendations:

* Since most of the delays were caused by Late return from Field Trips, it is recommended that the buses be rotated out to prevent breakdown i.e the buses going out for field trips should be on rotational basis.

* Heavy traffic is the most frequent reason for running late and hence either the roads be expanded to ease traffic or the number of vehicles plying that route should be regulated. Alternative routes may also be considered.

* An investigation into LITTLE RICHIE BUS SERVICE which is the bus company with the most breakdowns should be launched to understand the reason.

[Back To The Top](#New-York-City-Bus-Breakdowns---Data-Wrangling-with-Python)

---

## Author Information

- Twitter - https://twitter.com/Vycellous_Drum
- Website - https://richardtaracha.glitch.me/

[Back To The Top](#New-York-City-Bus-Breakdowns---Data-Wrangling-with-Python)


