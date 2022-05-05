# Disneyland Ride Wait Times Project

## Project Objective
The problem that I am aiming to solve through this project is which Disneyland rides should Disney focus their marketing efforts towards? In order to solve this problem, I have analyzed wait time data for Disneyland rides, finding the average wait time, the percentage of time that a ride has been open, and the minimum and maximum wait time values for each ride in a given time period. Ultimately, from this data, I have determined that Disneyland should focus their marketing efforts on rides with shorter wait times, greater percentages of time they are open, and smaller ranges between their maximum and minimum wait time; ultimately, this means that Disney should increase marketing efforts for "less popular" rides that are open over 90% of the time and that have less range between their maximum and minimum wait times. By marketing these kinds of Disneyland rides, Disney could potentially decrease the wait times for their most popular rides, increasing customer satisfaction, and increase park-goers' interest in their "less popular rides."

## Job Description
The job that I have selected as the inspiration and basis for this project was the Marketing Analytics & Optimization Internship with Disney. The role of this internship consisted of seeking marketing optimization opportunities for Disney Parks, Products, and Experiences through various media, as well as evaluating the current marketing strategies of for the business.

## Data Source
This Data was sourced from the following APIs:

Disneyland: https://queue-times.com/en-US/parks/16/queue_times.json

Disney California Adventure: https://queue-times.com/en-US/parks/17/queue_times.json

For Park Names: https://queue-times.com/en-US/parks.json

From the first two APIs, I was able to find data such as ride ids, ride names, last_updated fields (for both rides and ride wait times), ride wait times, and whether rides were open or not. In order to ensure that I had a robust collection of data to choose from, I ran my notebooks through DeepNote, where I scheduled data collection every hour at the 1 minute mark.

*** Note: For the sake of this project, I will be focusing primarily on my Disneyland rides data collection ***

## Notebooks
Here are the following notebooks that I used in the collection of my data and my analysis of the ride times:

Data Collection: 

The purpose of this Data Collection notebook is to make requests to the Disneyland Ride Wait Times API, parse through the data to access ride-specific information, and then compile the data into a data frame so it could be stored in a database.

Data Analysis:

The purpose of this Data Analysis notebook is to utilize SQL in order to access the database with the ride times and analyze the data, performing queries such as average wait time per ride, percent of time a ride is open, and maximum and minimum wait times in a given period. 

## Future Improvements
Some improvements I would like to make to this project are:
1. Collect more data from the Disney California Adventure API so that Disneyland and Disney California Adventure could be properly compared.
2. Implement a Lands Table so that the data could also be filtered by Lands, rather than just by ride and park.
