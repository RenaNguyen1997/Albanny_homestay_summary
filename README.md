# Albanny_homestay_summary
## Overview

This project is descriptive analytics, summarizing key insights of homestay business in Albany and identifying core elements contributing to suitable and economic property selection. The statistics will showcase my foundation in utilizing Excel, particularly VBA, to perform data wrangling and data mining skills. The final result is demonstrated as an interactive dashboard created via Tableau. 

The project's whole purpose is to provide the most suitable homestays for the viewer in terms of prices and value.

## Key skill demonstrated
* **Data cleaning and Data mining**: Extracted data from the original source, combining all statistics into one coherent file, handling missing data and outliers to create a suitable dataset for analysis and visualisation.
* **Exploratory Data Analysis (EDA)**: Identifying trends, patterns, and relationships in data.
* **Data Visualization**: Using Tableau to create interactive charts and graphs 
* **Excel (particularly VBA code)**: For querying databases, manipulating datasets, and performing calculations. 

## Table of contents
1. [Project setup](#project-setup)
2. [Project structure](#project-structure)
3. [How to run the project](#how-to-run-the-project)
4. [Key analysis and visualisation](#key-analysis-and-visualisation)
5. [Insights and findings](#insights-and-findings)

## Project setup
To run this project, you will need: 

* Access to the Tableau Desktop for visual reporting.
* Acess to Microsoft Excel and VBA window to save and manipulate downloaded data

## Project structure
* **Project overview**: The current document will describe the general structure of the project on Github and instruction on how to use each diffferent files to complete the descriptive analysis
* **How to clean data**: 
* **Dataset**: Within this project scope, the used data will be saved under .xlsm format, in a total of 4 different files, including 3 original files and 1 finalized dataset after cleaning and mining.\
Please find [Albany's most updated data](https://insideairbnb.com/get-the-data/) by clicking on the hyperlink

* **Dashboard**: The interactive dashboards incorporating the insights and results will be demonstrated via Tableau file under the name "" accordingly.

## How to run the project
*To obtain and clean original data before visualisation*
1. Downloading the neccessary data: In the Project structure, you can access the most updated data by clicking on the provided link under the section "Data source". Otherwise, please find the used data within this project scope by downloading 3 files in the Dataset folder: Listings, Reviews, and Calendar.
2. Cleaning the data:
Due to their size and large information, these files required extensive time to be cleaned and mined. After downloading the necessary dataset, please open the document "How to clean data" and view the detailed  step-by-step description.

*To obtain the ready data*\
The finalized dataset can be found under the name 'Dataset_official.xlsm' under the Dataset folder. 

*To visualize data*
1. Download the Tableau file under the name "Albanny_dasboard.tmb"
2. Merging data: Before visualizing, merging data between different files is required. Instead of manually doing it from Excel, Tableau can assist with the task ideally by joining the data based on similar columns between each file:
<p align="center">
<img src="https://github.com/RenaNguyen1997/image/blob/main/Albanny/Tableau_merge.PNG" width=70% height=50%>
</p>

## Key analysis and visualisation in Dashboard
* **Price summary:** Descriptive analytics on price by unit category and different room features
* **Lists:** A list of homestays with filter options for manually finding the desired homestay 

## Insights and findings
* Insights 1: By room category
  Staying in a private room will cost much less than renting the whole unit. 
  For private rooms, The low season is between April - and August, November and December.
  For the entire unit: The low season is from December to Jun

* Insight 2: By number and type of bathrooms
Properties providing private bathrooms will generally have higher prices than shared bathrooms. Furthermore, the more bathrooms there are, the higher the price.

* Insight 3: Number of people traveling 
Generally, the price will increase as the number of accommodations increases. However, the cost per person will be less as the number of people traveling increases until the total number exceeds five people, at which point the price will also increase.
