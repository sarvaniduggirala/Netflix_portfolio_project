# Netflix Data Analytics Project

## Table of Contents ##

1. Overview
2. Folder Structure
3. Data Cleaning in Excel
4. MySQL Database Integration
5. Power BI Dashboard Creation
6. Additional Insights and Details

## Overview

Welcome to my first portfolio project! In this project, I explored and analyzed the Netflix Titles dataset to derive meaningful insights and visualize trends using Data Analytics techniques. The journey involved data cleaning in Excel, SQL database manipulation, and creating an interactive Power BI dashboard.
* Data was taken from the Netflix Titles dataset.
* The dataset: netflix_titles.csv

## Folder Structure ##
* **/data:** Holds both raw and cleaned datasets.
* **/sql_queries:** Showcases SQL queries used for data consolidation.
* **/power_bi_dashboard:** Stores the Power BI files for the interactive dashboard.
* **/documentation:** Offers additional project documentation.

## Data Cleaning in Excel ##
I initiated the project by meticulously cleaning the raw Netflix Titles dataset in Excel. The process involved:

* Utilizing the Split Text to Columns tool to separate values in columns such as **'countries_released'**, **'listed_in'**, **'cast'**, and **'directors'** where multiple names were present.

* Creating a new column called **'duration_type'** by splitting the **'duration'** column, which contained different types (minutes and seasons).

*Before:*
  
![image](https://github.com/sarvaniduggirala/Netflix_portfolio_project/assets/158331818/0d495f3a-4aa6-4a91-bf99-1694f40a0222)

*After:*
  
![image](https://github.com/sarvaniduggirala/Netflix_portfolio_project/assets/158331818/c752dc7f-e628-4c2f-970e-f221b3180e44)


* Implementing the TRIM function to remove any unwanted spaces and Replaced blank cells with **'NULL'**
* Dividing the dataset into different workbooks for better organization.

![image](https://github.com/sarvaniduggirala/Netflix_portfolio_project/assets/158331818/9ad7f31d-c6ac-4bbd-acc9-fe050afcc046)

## MySQL Database Integration
Following the Excel cleaning phase, I imported the cleaned data into MySQL Workbench. However, to streamline the analysis, I noticed the need to pivot the tables. This involved consolidating non-null cells from multiple columns into a single column, paired with their respective **'show_id'** in the **'netflix_data'** database.

![image](https://github.com/sarvaniduggirala/Netflix_portfolio_project/assets/158331818/c6802c9e-3f63-496d-85e3-23d82002c6a2)

## Power BI Dashboard Creation 
With the pivoted data in place, I connected it to Power BI for visualization. 
### Overview Page
The "Overview" page of the Power BI dashboard is designed to provide a rich and insightful experience:
* **Area Chart:** Illustrates shows added by year using **'release year'** and **'show_id'**.
* **Stacked Column Chart:** Represents shows by **'rating'** using the **'show_id'**.
* **Bar Chart:** Displays the **top 10 genres** of shows based on the ***count*** of **'show_id'**.
* **Map Chart:** Highlights countries where shows are available, with the ***count*** of **'show_id'** reflected in bubble size.

  ![image](https://github.com/sarvaniduggirala/Netflix_portfolio_project/assets/158331818/dec650dc-abc2-4110-a71a-880284992f25)


### Single Title View Page
On the "Single Title View" page, I incorporated additional insights and details:
* **Slicer:** Allows users to filter between **'movies'** and **'TV shows'**.
* **Cards:** Provide quick access to essential information, including **'rating'**, **'release year'**, and a **'description'** of the selected movie/TV show.
* **Map Chart:** Visualizes countries where the selected movie/TV show is available.
* **Multi Row Cards:** Display comprehensive information on **'categories'**, **'directors'**, and **'cast'**.

![image](https://github.com/sarvaniduggirala/Netflix_portfolio_project/assets/158331818/be94d777-7672-4e02-a62e-95710401d30f)

## Project Highlights
This project is a showcase of my practical skills in data analytics.  Here's what I've done:

* **Cleaning Data:** I tidied up the Netflix Titles dataset using Excel. I split, trimmed, and organized the data to make it neat and ready for analysis.

* **Database Management with MySQL:** I smoothly moved the clean data into MySQL Workbench. There, I reorganized and simplified things to make it easier to work with.

* **Dynamic Power BI Visualizations:** Crafted an engaging Power BI dashboard with dynamic visual elements such as area charts, stacked column charts, bar charts, and map charts. These visuals help in providing insightful perspectives.

* **SQL Query Optimization:** Utilized SQL queries to enhance database efficiency, consolidating tables and improving overall query performance.

This project is my way of showing how I handle data – making it clean, understandable, and telling a story with it.Please take a look around the dashboard, and you might discover some interesting things about Netflix titles!

[Netflix Dashboard](https://stuconestogacon-my.sharepoint.com/:u:/g/personal/sduggirala9126_conestogac_on_ca/EaEBhL7zEJFJpwP0vk7NFxkBoiys9OCpMiHf-kBGu35XnA?e=LXDeEc)

Thanks for joining me on this project! 
