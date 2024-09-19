# Battle of Neighborhoods: Coffee Shop Location Analysis in Vaughan, Canada

## Project Overview

This data science project analyzes neighborhoods in Vaughan, Canada to determine the optimal location for opening a new coffee shop. It's part of the IBM/Coursera Applied Data Science Capstone course, demonstrating the practical application of data analysis and machine learning techniques to solve real-world business problems.

## Table of Contents

1. [Introduction](#introduction)
2. [Business Problem](#business-problem)
3. [Data Sources](#data-sources)
4. [Methodology](#methodology)
5. [Analysis](#analysis)
6. [Results](#results)
7. [Discussion](#discussion)
8. [Conclusion](#conclusion)
9. [Dependencies](#dependencies)
10. [How to Use](#how-to-use)

## Introduction

Choosing the right location is crucial for the success of any new business. This project leverages data science techniques to provide insights for entrepreneurs looking to open a coffee shop in Vaughan, Canada.

## Business Problem

The main objective is to identify neighborhoods in Vaughan (focusing on the boroughs of North York, East York, and York) that currently lack coffee shops and have characteristics that suggest they could support a successful new coffee shop business.

## Data Sources

1. Canada Postal Code data: Scraped from [Wikipedia](https://en.wikipedia.org/wiki/List_of_postal_codes_of_Canada:_M)
2. Geospatial coordinates: Obtained from [Cocl.us Geospatial Data](http://cocl.us/Geospatial_data)
3. Venue data: Collected using the Foursquare API

## Methodology

1. **Data Collection and Preprocessing**: 
   - Web scraping of postal code data
   - Merging with geospatial coordinates
   - Collecting venue data using Foursquare API

2. **Exploratory Data Analysis**:
   - Visualizing neighborhoods using Folium maps
   - Analyzing venue categories in each neighborhood

3. **Feature Engineering**:
   - One-hot encoding of venue categories
   - Calculating mean frequency of venue categories per neighborhood

4. **Clustering**:
   - Applying K-means clustering to group similar neighborhoods
   - Visualizing clusters on a map

5. **Results Analysis**:
   - Examining characteristics of each cluster
   - Identifying promising neighborhoods for a new coffee shop

## Analysis

The analysis involved several key steps:

1. Identifying neighborhoods without existing coffee shops
2. Exploring the most common venue types in these neighborhoods
3. Clustering neighborhoods based on their venue profiles
4. Visualizing the clusters on an interactive map

## Results

The clustering analysis resulted in 5 distinct neighborhood clusters. Two clusters were identified as particularly promising:

- **Cluster 0**: Includes neighborhoods such as Parkview Hill, Glencairn, and Woodbine Heights
- **Cluster 3**: Contains neighborhoods like Parkwoods, Caledonia-Fairbanks, and Weston

These clusters showed a good balance of various venue types, suggesting a diverse and active local scene that could support a new coffee shop.

## Discussion

While both Cluster 0 and Cluster 3 showed promise, Cluster 0 was deemed more suitable due to the closer proximity of its neighborhoods. Within Cluster 0, the **Downsview** neighborhood stood out as a particularly attractive option for a new coffee shop.

## Conclusion

Based on the available data and analysis, **Downsview** in Vaughan emerges as a promising location for opening a new coffee shop. However, it's important to note that this analysis has limitations. Factors such as population density, foot traffic, and local economic conditions were not included in this study and should be considered before making a final business decision.

## Dependencies

- Python 3.x
- pandas
- numpy
- matplotlib
- seaborn
- beautifulsoup4
- requests
- folium
- scikit-learn
- geocoder

## How to Use

1. Clone this repository:
```git clone https://github.com/your-username/vaughan-coffee-shop-analysis.git```
2. Navigate to the project directory:
```cd vaughan-coffee-shop-analysis```
3. Install the required dependencies:
```pip install -r requirements.txt```
4. Open and run the Jupyter notebook:
```jupyter notebook Battle_of_Neighborhoods_part_3.ipynb```

Note: You'll need to obtain your own Foursquare API credentials to run the venue analysis portion of the notebook. Replace the placeholder credentials in the notebook with your own.

## Contributing

Contributions to improve the analysis or extend the project are welcome! Please feel free to fork the repository, make your changes, and submit a pull request.
