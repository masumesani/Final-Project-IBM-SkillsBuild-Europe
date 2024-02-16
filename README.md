# Finding Your NYC Sweet Spot: Balancing Budget and Vibe with Airbnb Data
# 📝 Table of Contents
- [About](#about)
- [Business Understanding](#business-understanding)
- [Data Understanding](#data-understanding)
- [Visualization and Result](#visualization)
- [Technologies](#techs)
- [Setup](#setup)
- [Approach](#approach)
- [Status](#status)
- [Credits](#credits)

## About <a name="about"></a>
This th Final Project presented by IBM-SkillsBuild-Europe for Programme in Data Analytics.

**Project objectives are :**
- Data Cleaning.
- Data Transformation.
- Data Visualization.
  
**Project Summary**
- Develop Python scripts for data transformation, focusing on cleaning and preprocessing data for analysis. Tasks include managing missing values, formatting, normalization.
- Conduct exploratory data analysis and apply analytical methods to real-world datasets using Python libraries such as Pandas, Numpy.
- Utilize dataframes to manipulate data, generate data summaries, comprehend data distributions, conduct correlation analyses, and establish data pipelines.
- Utilize Python libraries, including Matplotlib, Seaborn to implement compelling data visualization techniques and plots that narrate a captivating story.
- Generate various chart types, such as line graphs, area plots, histograms, bar charts, pie charts, box plots, and scatter plots.
- Perform data analysis and visualization in a Jupyter Notebook
- The combination of Jupyter Notebooks and CSV file facilitates a flexible and transparent workflow for data processing, analysis, and visualization in this Python project.

## Business Understanding <a name="business-understanding"></a>
Unveiling Airbnb Listing Trends for Informed Hosting Strategies<br/>

**Executive Summary:**

Understanding market trends and customer preferences is crucial for success in the competitive Airbnb landscape. This analysis leverages a sample Airbnb dataset to provide valuable insights into the availability of different room types, the impact of cancellation policies, and pricing strategies across neighborhoods.

**Problem:**

Hosts need data-driven insights to make informed decisions about their listings, including:

1. Which room types are most in demand?<br/>
2. How do cancellation policies affect bookings?<br/>
3. Which neighborhoods offer the highest rental potential?<br/>

**Objective:**

This analysis aims to:

1. Quantify the distribution of various room types (entire homes, private rooms, shared rooms,..).<br/>
2. Identify the room type with the strictest cancellation policy, potentially impacting booking rates.<br/>
3. Analyze average rental prices by neighborhood to reveal lucrative areas for Airbnb hosts.<br/>



## Data Understanding <a name="data-understanding"></a>
**Data Sources:** 

For this project, we utilize the Airbnb Open Data set hosted on Kaggle: https://www.kaggle.com/datasets/arianazmoudeh/airbnbopendata <br/>
This dataset offers a robust collection of information on Airbnb listings across NYC. Key features include: <br/>
- Listing features: Neighborhood, room type, price, availability, reviews, service fee, cancellation policy, and house rules.
- Location data: Neighborhood, latitude, longitude.
- Calendar data: Availability and price per date.
- Host data: Host ID and other relevant information (optional).
  
**Why This Dataset:**

The Airbnb Open Data presents several advantages for our project:

- Publicly available: Freely accessible, promoting open-source analysis and reproducibility.
- Comprehensive: Covers crucial aspects like location, listing details, and pricing information.
- Sizeable: Contains a substantial number of listings, enabling statistically significant insights.
> [!NOTE] 
> Based on link provided for this project, data set is about New York city, since there is no counties as brookln and manhatan, it seems they are unintentional data entry error which can affect overall data quality and analysises.<br/> 
> As such, I decided to address it and update my data set accordingly. Although mentioned correction in average price calculation against Neighbourhood Group does not show changes but in analysing booked days we can see different results.<br/> 
> There are also 13 row of with minimum night of negative value which I catch them by running  AirbnbData[AirbnbData['minimum_nights']<0] but I decided to go with them and filter them further down the road.

## Visualization and Result <a name="visualization"></a>
### Key Findings

1.The examined dataset included listings offering entire homes/apartments, private rooms, shared rooms and hotel rooms.<br/>
2. Entire homes/apartments possessed the strictest cancellation policy, potentially influencing booking decisions.<br/>
3. Queens emerged as the most expensive neighborhood, with an average rental price higher than Brooklyn and Manhattan. <br/>
4. It seems people renting through Airbnb in New York city have demand for renting a Shared Room more than Entire home/apt or Private Room. Therefore avarege price for this type of room hold the sencond place in matter of most expensive ones.<br/>
5. There are 1032 records for Shared Room that their price are higher than 670 $ whcih is avarage price for Hotel Room category.<br/>
6. Hotel Rooms average price for renting from Airbnb is 666.39 $ which seems higher than normal price in same year. <br/>
7. According to https://www.statista.com/ "The average daily rate of hotels in New York appears to be much higher in the fourth quarter of the year, reaching 389 U.S. dollars in 2016".<br/>
8. It seems more expensive Hotels tend to offer thier rooms on Airbnb, where they can ask for higher price.<br/>
9. Chosing which type of room is more matter of taste than matter of affordability. As there are not that much of difference in average price of all room types. <br/>
10. Stanten Island has most records of bookings.
11. Lighthouse Hill is the cheapest neighborhood with average price of $107.67.

### Business Implications

These findings offer valuable insights for Airbnb hosts:<br/>

1. Consider diversifying offerings by including different room types based on demand.<br/>
2. Evaluate cancellation policies for potential trade-offs between flexibility and booking security.<br/>
3. Prioritize listing optimization in premium neighborhoods like Queens to capitalize on higher rental potential.<br/>

### Visualization
Please checck https://github.com/masumesani/Final-Project-IBM-SkillsBuild-Europe/blob/main/Visualizations%20.md

## Technologies <a name="techs"></a>
- Python and Python libraries like Numpy, Pandas, Matplotlib, Seaborn
- Anaconda
- Jupyter Notebook 

## Setup <a name="setup"></a>
- Download or clone repository
- Load Anaconda
- Open Jupyter Notebook
## Approach <a name="approach"></a>
The analysis examined a sample Airbnb dataset, focusing on room type, cancellation policy, and neighborhood pricing.
Descriptive statistics were employed to calculate counts, averages, and identify the most expensive neighborhood.
## Status <a name="status"></a>
Completed
## Credits <a name="credits"></a>
- This is the final project for Programme in Data Analytics | IBM | SkillUp | 2023 for more info look at https://skills.yourlearning.ibm.com/activity/PLAN-140B7B12702D?focuslmsId=URL-279FC6427A2F <br/>
- Dataset Source provided by  https://www.kaggle.com/datasets/arianazmoudeh/airbnbopendata

