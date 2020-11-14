# Descriptive-Analysis-of-Ride-Sharing-App-Prices- (Uber & Lyft)
---

> Author: Richard Taracha

> Date: 14/11/2020

![UberLyft-1-1200x402](https://user-images.githubusercontent.com/67068918/99152615-e5b86300-26b3-11eb-80ff-a8128f721080.png)

---

### Table of Contents
Sections headers used to reference locations of each destination:

- [Understanding The Context](#understanding-the-context)
- [Project Deliverable](#project-deliverable)
- [Recording the Experimental Design](#recording-the-experimental-design)
- [Summary Of Findings](#summary-of-findings)
- [Recommendations](#recommendations)
- [Author Information](#author-information)

---

## Understanding The Context

Come up with a descriptive analysis report to help a Ride Sharing Startup coming into the space, understand the various patterns on how pricing works for the existing ride sharing company. 

I'm able to access some real-time data from Uber & Lyft's API and weather data from a Weather API conditions. I built a custom application in Scala to query data at regular intervals and saved it to DynamoDB. The queried cab ride estimates are done after every 5 mins and weather data after every 1 hr. 

The cab ride data covers various types of cabs for Uber & Lyft and their price for the given location. Weather data contains weather attributes like temperature, rain, cloud, etc for all the locations taken into consideration.

Given a dataset, I wrote sql queries to perform descriptive analysis highlighting key insights that would be helpful in helping the startup develop a new product. 

#### Technologies and Tools

- Python Programming Language
- sqlite
- SQL
- Google Colab Notebook

[Back To The Top](#New-York-City-Bus-Breakdowns---Data-Wrangling-with-Python)

---

## Project Deliverable
Deliverable is an SQL notebook with my data analysis in SQL:

* Notebook name: Descriptive Analysis of Ride Sharing App Prices.ipynb

Datasets:
Weather Dataset URL = https://bit.ly/cabsweatherdata

Cabs Dataset URL = https://bit.ly/cabsdataset

Dataset Glossary:
* Cab Rides Dataset
1. distance: distance between source and destination. 
2. cab_type: Uber or Lyft
3. time_stamp: time when data was queried
4. destination: destination of the ride
5. source: the starting point of the ride
6. price: price estimate for the ride in USD
7. surge_multiplier: the multiplier by which price was increased, default 1
8. unique identifier
9. product_id: uber/lyft identifier for cab-type
10. name: Visible type of the cab eg: Uber Pool, UberXL

* Weather Dataset
1. temp: Temperature 
2. location: Location name
3. clouds: Clouds
4. pressure: pressure in mb
5. rain: rain in inches for the last hr
6. time_stamp: time when row data was collected
7. humidity: humidity in %
8. wind: wind speed in mph

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


