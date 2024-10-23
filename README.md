# Identify On-Off Properties
The Off-Market Property Identifier helps real estate professionals, investors, and researchers find properties not currently listed on the market. By cross-referencing data from the Multiple Listing Service (MLS) with county assessor records, it identifies off-market properties, offering a valuable resource for uncovering potential opportunities.

## Overview:
>  From assessor records, filtering invested properties and then breaking down those results down into flipped properties. Distinguishing between ON and Off markets deals of each filter is the last step.

## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Setup](#setup)
* [Usage](#usage)
* [Project Status](#project-status)
* [Room for Improvement](#room-for-improvement)
* [Contact](#contact)
<!----------------->

## General Information
- The scope of this project is to focus on threen key purposes: 
    1. Finding out invested properties from  the main dataset.
    2. Checking whether an invested properties was a flip one or not.
    3. From step two, Seperating Sold On Vs. Off Market properties by comparing properties ID to MLSers' or 1st American Listing's properties ID.
- Main datset includes: ds_assessor_records.csv
- MLS listings file includes: red_chicago_property_listings.csv, red_dallas_property_listings.csv,
and red_denver_property_listings.csv. 
- First American file includes: ds_listings.csv.
- The project is broken down into city as the request of Mr.Scott. 

## Technologies Used
- Python 3.9.7
- Pandas 1.3.4
- Numpy 1.20.3
- plotly 5.6.0

## Usage
- Four CSV files (private) are needed to run the Compare_MLSes_to_1stAmerican.ipynb are: 
    - ds_assessor_records.csv
    - red_chicago_property_listings.csv
    - red_dallas_property_listings.csv
    - red_denver_property_listings.csv
    - ds_listings.csv
- Note: Due to the large dataset size, only some useful columns were read to be used for this analysis. 

## Project Status
Project is:  _completed_ 

## Room for Improvement
- What we think this project can be improve is to identify what are those negative values of Id columns from the 4 files, so we can decide to either filter them out or include them while comapring. 
- This project can also be done faster using SQL code on data warehouses. 
