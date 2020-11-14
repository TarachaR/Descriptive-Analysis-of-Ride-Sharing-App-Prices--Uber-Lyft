# Descriptive-Analysis-of-Ride-Sharing-App-Prices-(Uber & Lyft)
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

The cab ride data covers various types of cabs for Uber & Lyft and their price for the given location. Weather data contains weather attributes like temperature, rain, cloud, etc for all the locations taken into consideration.

#### Technologies and Tools

- Python Programming Language
- sqlite
- SQL
- Google Colab Notebook

[Back To The Top](#>Date:-14/11/2020)

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
6. Data Analysis with SQL

Given a dataset, I wrote sql queries to perform descriptive analysis highlighting key insights that would be helpful in helping the startup develop a new product.  

As a start while performing data analysis, I derived the following questions from the given datasets: 
1. When do prices hit a high during 3 periods of the day?
2. Get a feel of average pricing for a single day, select a random day and break it into periods of the day: 
* Midnight to early morning (12am - 6am)
* Early morning to midday (7am - 12pm)
* Early afternoon to late evening (1pm - 6pm)
* Late evening to midnight (7pm - 11pm)
3. What is the average price charged by each cab per distanced travelled,, minimum price charged by each cab per distanced travelled, maximum price charged by each cab per distanced travelled


[Back To The Top](#New-York-City-Bus-Breakdowns---Data-Wrangling-with-Python)

---

## Summary Of Findings

The following are the prices for Lyft:

- overall average of 16.54, overall minimum 2.5, overall maximum 97.5
- average 17.3, minimum 2.5, maximum 97.5 from midnight to 6 AM
- average 17.35, minimum 2.5, maximum 89.0 from 7 AM to 12 PM
- average 17.33, minimum 2.5, maximum 92.0 from 1 PM to 6 PM
- average 17.37, minimum 2.5, maximum 92.0 from 7 PM to 11 PM

The following are the prices for Uber:

- overall average of 15.79, overall minimum 4.5, overall maximum 89.5
- average 15.80, minimum 4.5, maximum 81.5 from midnight to 6 AM
- average 15.75, minimum 4.5, maximum 80.5 from 7 AM to 12 PM
- average 15.80, minimum 4.5, maximum 89.5 from 1 PM to 6 PM
- average 15.81, minimum 4.5, maximum 76.0 from 7 PM to 11 PM
- Minimum distance is 0.02, maximum distance is 7.86.

For distance 0.00-1.96: Lyft has average price 14.07, minimum price 2.5, and maximum price 65.0. Uber has average price 13.37, minimum price 4.5, and maximum price 61.5.

For distance 1.97-3.93: Lyft has average price 19.24, minimum price 2.5, and maximum price 92.0. Uber has average price 17.14, minimum price 6.0, and maximum price 80.5.

For distance 3.94-5.89: Lyft has average price 25.54, minimum price 3.0, and maximum price 97.5. Uber has average price 22.33, minimum price 7.5, and maximum price 87.0.

For distance 5.90-7.86 Lyft has average price 30.1, minimum price 10.5, and maximum price 65.0. Uber has average price 26.10, minimum price 10.0, and maximum price 89.5.

[Back To The Top](#New-York-City-Bus-Breakdowns---Data-Wrangling-with-Python)

---

## Recommendations
The Ride-Sharing Startup management team can use this information as a starting point then later adjust accordingly based on user feedback.

[Back To The Top](#New-York-City-Bus-Breakdowns---Data-Wrangling-with-Python)

---

## Author Information

- Twitter - https://twitter.com/Vycellous_Drum
- Website - https://richardtaracha.glitch.me/

[Back To The Top](#New-York-City-Bus-Breakdowns---Data-Wrangling-with-Python)


