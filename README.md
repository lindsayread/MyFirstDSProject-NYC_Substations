# **Metis Project 1 - Summer 2020**

## About:

In this project, I worked with three of my fellow Metis classmates to provide insight to WomenTechWomenYes (WTWY) as to when and where they should focus on deploying their street team in order to get the most amount of signatures of people who are interested in attending their gala, which is geared especially towards women in technology.

## Project Goals:
We saught to perform EDA on the MTA Subway data to investigate the following:

1. Which subway stations are the busiest?
2. What time of the day are these stations busiest?
3. What day of the week are they busiest?
4. Which stations do we want to target based on the likelihood of our target audience (people interested in technology, especially women) being at these subway stations?

## Process:

Once we had a general idea of the insights we wanted to discover, we needed to find a dataset (or several datasets) that we could analyze to transform these insights. The first, and main, dataset that we used is [Turnstile Data](http://web.mta.info/developers/turnstile.html), which contains ridership information for the MTA Subways in New York City for all weeks from 10/18/14 to the current week. We decided to look specifically at the 2 months leading up to the gala (April and May 2019), as people riding the subway during these dates are more likely to still be around in a month or two when the gala is taking place.

My major contribution to the group project was to investigate which stations were nearby major tech companies and Universities. After finding the GPS coordinates of NYC's 5 major tech companies and top 5 technology driven Universities, I programmatically calculated the haversine (great cicle) distance between each station and each tech company and university. Once I had these distances for each station with respect to the companies and universities, I engineered a new feature that calculated the total number of tech companies and/or universities within walking distance (which I defined as 1 km or less). I then identified the stations that would be optimal for our target group: 3rd Av, Astor Place, 8th St, 125th St, Union Square, 14th St-Union Square, Broadway-Lafayette St, Bleecker St.

We then combined this knowledge with the insights we gathered from the rest of the data (the 10 stations with the highest total overall traffic, the days of the week with the highest traffic, and the time of day with the highest traffic) to determine the overall optimal placement of the WTWY street team.

## Results:

Through triumphant teamwork, my team and I were able to determine that the most optimal placement of the WTWY street team was at the 14 St-Union Sq. station as this station is one of the top 5 busiest MTA stations overall and it is within 1 km of several major tech companies and universities. In terms of the optimal day and time for the street team to be deployed, we concluded that weekday evenings (between 6 and 8 pm) would be the best as these are the busiest times of the day.

## Files:

In this project, you will find the files used to gather the data, create visualizations, and a PDF of our presentation.

### Slideshow PDF:

PDF of our Google Slides presentation.

[MTA_Project_1.pdf](https://github.com/lindsayread/MyFirstDSProject-NYC_Substations/blob/master/MTA_Project_1.pdf)

### Code Files:

1. Main code file: In this file, you will find code for our data acquisition, EDA, and visualizations.

[final_code.ipynb](https://github.com/lindsayread/MyFirstDSProject-NYC_Substations/blob/master/final_code.ipynb)

2. Distance from Stations to Universities and Tech Companies code file: In this file, you will find code for mapping the distance from each station to each tech-focused university and major tech centers, as well as a count of how many tech centers and universities are within 1 km of each subway station.

[subway_locations_tech_and_universities.ipynb](https://github.com/lindsayread/MyFirstDSProject-NYC_Substations/blob/master/subway_locations_tech_and_universities.ipynb)

## Data:

[Ridership Data](http://web.mta.info/developers/turnstile.html)

[Station Locations Data](https://data.ny.gov/Transportation/NYC-Transit-Subway-Entrance-And-Exit-Data/i9wp-a4ja)

## Skills:

- Python 
- Pandas
- EDA
- Matplotlib and seaborn visualizations
