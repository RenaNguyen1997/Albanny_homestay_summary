# How to clean data in the dataset folder

## Overview 
The instructions aim to verify how to use the "Code.xlsm" file to clean and mine data for each dataset to obtain the desired final data and further exploration. 

## Structure
1. Structure of general dataset
2. How to clean "Listings" dataset
3. How to clean the "calendar" and "review" dataset

## Structure of general dataset

You can access the most updated dataset via the below link [Albany's most updated data](https://insideairbnb.com/get-the-data/)

The data is updated every three months for different cities and countries. For practice, I only look into the Albany dataset 

The data includes three different files: 
| **Files** | **Number of rows** | **Number of columns** | **Details** |
| --- |          ---|           ---|---     |
| Listings| 4230| 72| Including the information of hosts and their homestay as well as all types of scores and reviews from the beginning until now|
| Reviews| 22,556| 2 | Id of the homestay and all of its reviews in text forms|
| Calendar| 143,811 | 6 | Future price and availability for 2024 and 2025|

## How to clean the "Listings" dataset
Among the three files, "Listings" contains the most valuable insights. Though many columns contain different data types, they can be summarized into four groups.
* **Group 1**: General information about the hosts and their homestay
* **Group 2**: Homestay's main features and price
* **Group 3**: Different theme of score for each homestay
* **Group 4**: General information on the reviews each homestay earns since the beginning

The cleaning process will include two primary stages: Narrowing and Cleaning 
#### *<ins>Narrowing</ins>*

Considering the project's main aim as **the most suitable and qualified homestay**, I will first **narrow** the list of homestays to analyze before understanding the price pattern. The homestays must satisfy the following criteria to continue for further analysis:

***1. Verified identification:*** 
The identification of the host is vital to ensure the **safety** of the stay. Hence, only the host with the verified identification will be included in the list. The purpose is achieved by **filtering out** those that **"host_identify_verfiy"** is **"no"**

***2. Columns with necessary data***
With the current dataset:
Group 2: Have the most impact on price patterns, 
Group 1: Be essential for creating the second dashboard (Suggest homestay for the viewer). 

Hence, all columns in Group 2, together with the name of the host and homestay in Group 1 and the general review score in Group 3, will be extracted into a separate file for further cleaning. 

*"Listings" will now contain only **13 columns** instead of 72 columns.*

#### *<ins>Cleaning</ins>*
The narrow process is finished. We can now move on to cleaning the files:

***1. Checking for duplicates:***\
Duplications can be removed easily by utilizing Excel's existing **"Remove Duplicates"** feature

***2. Re-organise type of data:***\
While most columns seem ready for analysis and visualization, the "bathroom" column does not satisfy the Normal Form of data analysis when a cell contains two values: the number of bathrooms and the Type of bathrooms. Consequently, further cleaning for "Listings" is required.

Though this can quickly be done by utilizing the existing features of Excel "Text to Columns," I would like to create a **ready function** that can be **repeatedly applied to all of the future data**, considering the source of data also includes information of other countries and cities other than Albany. Hence, I am going to use VBA for this cleaning process. The code that is desired for cleaning purposes can be found in "Code.xlms" in this repository. 

The code will include 3 steps\
(1) Split the number and the text into two columns\
(2) Reduce the null data on bathroom types by setting certain conditions to decide bathroom types (based on detailed instructions of the original dataset)\
(3) Generalize the bath type into private and shared for better visualization

## How to clean the "calendar" and "review" dataset
These two files are quite simple and straightforward, without complicated columns and information. Hence, for these two files, I will only proceed with basic cleaning steps: Checking duplicates and null data while maintaining the rest of the data\

***1. Checking duplicates:***\
Utilizing the "Remove Duplicates" feature of Excel

***2. Checking null:***\
After checking the potential of having null data via the filter option, the dataset is cleaned with a clear category and no null data.

## Conclusion
In summary, most of the cleaning and mining efforts focus on the "Listings" dataset via two primary processes: Narrowing down and Cleaning. 
We only proceeded with the basic cleaning stage for the remaining dataset, which included checking null and duplicates. 
The dataset is now ready to use for further analysis

The final dataset is named "dataset_official.xlsx"









