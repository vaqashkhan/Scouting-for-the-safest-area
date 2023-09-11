# Scouting-for-the-safest-area
# London Borough Safety and Neighborhood Exploration

## Abstract
This project aims to assist individuals, especially expats considering relocating to London, in selecting the safest borough in London based on crime statistics. Additionally, it explores the neighborhoods within the chosen borough to identify the 10 most common venues in each neighborhood. The project employs k-means clustering to group neighborhoods with similar characteristics. This tool is highly valuable for those seeking a secure and convenient place to live in London.

## Introduction
### Background
Relocating is a significant life event, often prompted by various factors such as career opportunities, lifestyle changes, or personal preferences. For those moving to a new location, especially a bustling metropolis like London, several critical considerations come into play. Among these, safety, location, neighborhood ambiance, and accessibility to essential amenities are paramount.

- **Safety**: Feeling secure in your new home is fundamental to your well-being and enjoyment of your surroundings.

- **Location**: The adage "location, location, location" holds true; it's crucial to choose a place that aligns with your lifestyle and needs.

- **Neighborhood**: The atmosphere and amenities in your chosen neighborhood can greatly impact your day-to-day life.

- **Accessibility**: Proximity to essential infrastructure such as roads, public transport, parks, schools, and more is essential for a comfortable life.

### Problem
This project addresses the need to identify the safest borough in London by analyzing historical crime data. While the crime data used in this project dates from 2008 to 2016, it provides valuable insights. Moreover, the project extends its analysis to explore neighborhoods within the safest borough, identifying the most common venues in each neighborhood. This information can guide individuals considering relocation to make informed decisions about where to settle in London.

## Methodology Used
### Data Acquisition
Data acquisition is the first step in our project, involving gathering, filtering, and cleaning data from various sources.

#### Data Sources:
1. **London Crime Data (2008-2016)**: We obtained crime data from Kaggle, focusing on the year 2016 as the latest available data. This dataset includes information such as crime categories, locations, and timestamps.

   - **Columns**:
     - lsoa_code: Code for Lower Super Output Area in Greater London.
     - borough: Common name for London borough.
     - major_category: High-level categorization of crime.
     - minor_category: Low-level categorization of crime within the major category.
     - value: Monthly reported count of categorical crime in a given borough.
     - year: Year of reported counts, 2008-2016.
     - month: Month of reported counts, 1-12.

   - **Source**: [London Crime Data on Kaggle](https://www.kaggle.com/jboysen/london-crime)

2. **London Borough Information**: We scraped data from Wikipedia, which includes details about the 33 London boroughs, categorizing them as Inner or Outer London, noting their status (e.g., Royal, City), local authorities, political control, and more.

   - **Columns**:
     - Borough: Names of the 33 London boroughs.
     - Inner: Categorization as Inner or Outer London borough.
     - Status: Categorization as Royal, City, or other borough.
     - Local authority: The local authority assigned to the borough.
     - Political control: The political party that controls the borough.
     - Headquarters: Headquarters of the boroughs.
     - Area (sq mi): Area of the borough in square miles.
     - Population (2013): The population in the borough recorded during 2013.
     - Co-ordinates: Latitude and longitude of the boroughs.
     - Nr. in map: A unique number for visual representation on a map.

   - **Source**: [London Borough Information on Wikipedia](https://en.wikipedia.org/wiki/List_of_London_boroughs)

3. **Neighborhood Data (Royal Borough of Kingston upon Thames)**: To explore neighborhoods within the safest borough, we gathered data from a Wikipedia page specific to the Royal Borough of Kingston upon Thames.

   - **Columns**:
     - Neighborhood: Name of the neighborhood in the borough.
     - Borough: Name of the borough.
     - Latitude: Latitude of the borough.
     - Longitude: Longitude of the borough.

   - **Source**: [Neighborhood Data in Kingston upon Thames on Wikipedia](https://en.wikipedia.org/wiki/List_of_districts_in_the_Royal_Borough_of_Kingston_upon_Thames)

## Getting Started
Follow these steps to use this project effectively:

1. **Data Gathering**: Ensure you have access to the required data sources mentioned above.
2. **Data Preprocessing**: Clean and preprocess the data as necessary to prepare it for analysis.
3. **Exploratory Data Analysis (EDA)**: Explore the London crime data to identify the safest borough based on crime statistics.
4. **Neighborhood Exploration**: Analyze and visualize neighborhoods within the chosen safest borough.
5. **K-means Clustering**: Apply k-means clustering to group neighborhoods based on common venues.
6. **Decision Making**: Use the insights gained to make informed decisions about selecting a safe and suitable borough for relocation in London.

Feel free to customize and expand upon this project to adapt it to other locations with adequate data that meet the model's preconditions.

## Disclaimer
The crime data used in this project is based on historical information up to the year 2016. It is essential to consider that crime rates may have changed since then. Make sure to consult up-to-date sources and consider various factors when making decisions related to relocation.

Happy exploring and best of luck with your relocation plans in London!
