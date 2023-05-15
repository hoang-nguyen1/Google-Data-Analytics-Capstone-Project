# Google Data Analytics Capstone Project

---

## Background
In 2016, Cyclistic launched a successful bike-share offering. Since then, the program has grown to a fleet of 5,824 bicycles that are geotracked and locked into a network of 692 stations across Chicago. The bikes can be unlocked from one station and returned to any other station in the system anytime. Until now, Cyclistic’s marketing strategy relied on building general awareness and appealing to broad consumer segments. One approach that helped make these things possible was the flexibility of its pricing plans: single-ride passes, full-day passes, and annual memberships. Customers who purchase single-ride or full-day passes are referred to as casual riders. Customers who purchase annual memberships are Cyclistic members.

---

## 1. Ask

***Business Question:***

How do annual members and casual riders use Cyclistic bikes differently?

***Key Stakeholders:***

* Lily Moreno
* Cyclistic marketing analytics team
* Cyclistic executive team

***Business Task:***

Use the data to explore and gain insights on how annual members and casual riders use bikes differently. From trends and insights, assist the team to implement marketing strategies aimed at converting casual riders into annual members.

---

## 2. Prepare

The data include information about Cyclistic's historical trip and customers' patterns in bike usage. It is obtained between April 2022 and March 2023 (12 months).

Link: [Data Source](https://divvy-tripdata.s3.amazonaws.com/index.html)

---

## 3. Process

Due to large amount of data and flexbility of R language, I will process the data with R Studio to work with the data more efficiently. This will be applied to data cleaning, analysis, and visualization.

### Data Preparation

* Libraries: tidyverse, lubridate, ggplot2
* Data are stored in CSV format and imported separately by months
* Checked data columns for name consistencies
* 12 months of data are merged into a single dataframe

### Date Cleaning

* Created additional columns (date, month, day, year, and day of week) for data analysis
* Removed start_lat, start_lng, end_lat, and end_lng columns from the data
* Got rid of missing values using `na.omit()`
* Created a ride length column in minutes with `difftime()`
* Converted the ride length column into numeric
* Removed and filtered the data so that it does not include values with negative or zero ride lengths
* Ordered the day of week column

---

## 4. Analyze

The analyze phase will explore the question "How do annual members and casual riders use Cyclistic bikes differently?" by performing descriptive statistical analysis and aggregating the data with group by to extract trends from bike users.

### Descriptive analysis

* Calculated the mean, median, min, and max on ride length column
* For each member types, I explored the average, min, and max ride length

### Data aggregation

* Explored the members type by looking at the count between annual vs. casual members
* Count number of each bikes type
* Group by members and bikes type to find to total count
* Count number of rides of weekday based on members type
* Calculated the average ride length by bike and member type
* Calculated the average of ride length for each member types based on week day

---

## 5. Share
After analyzing the data, I visualize the data with pie chart and bar graphs to discern the differences in bike patterns visually between annual and casual members. Data visualization is a powerful tool to draw insights quickly













