# ETL_Historical_Weather_Forecast

This Coursera project is from the course: Hands-on Introduction to Linux Commands and Shell Scripting, which is a part of the 13 course series: IBM Data Engineering Professional Certificate.

The goal of this project is to practice the skills of data engineering, specifically Extract, Transform, and Load (ETL) processes using Linux shell scripting skills.

### Scenario
You've been tasked by your team to create an automated Extract, Transform, Load (ETL) process to extract daily weather forecast and observed weather data and load it into a live report to be used for further analysis by the analytics team. As part of a larger prediction modelling project, the team wants to use the report to monitor and measure the historical accuracy of temperature forecasts by source and station.

As a proof-of-concept (POC), you are only required to do this for a single station and one source to begin with. For each day at noon (local time), you will gather both the actual temperature and the temperature forecasted for noon on the following day for Casablanca, Morocco.

At a later stage, the team anticipates extending the report to include lists of locations, different forecasting sources, different update frequencies, and other weather metrics such as wind speed and direction, precipitation, and visibility.

Data source
For this practice project, you'll use the weather data package provided by the open source project wttr.in, a web service that provides weather forecast information in a simple and text-based format. For further information, you can read more about the service on its GitHub Repo.

First, you'll use the curl command to scrape weather data via the wttr.in website. For example, to get data for Casablanca, enter:

curl wttr.in/casablanca

which prints the following to stdout:
![image](https://github.com/prateekrana24/ETL_Historical_Weather_Forecast/assets/88931114/2a7cfe95-251f-4da8-81f2-ebfd6d6a1de9)

### Learning Objectives
After completing this practice project, you will be able to apply your new shell scripting skills in a real-world scenario to:

Download raw weather data
Extract data of interest from the raw data
Transform the data as required
Load the data into a log file using a tabular format
Schedule the entire process to run automatically at a set time daily

### Weather Reporting Tasks
You must extract and store the following data every day at noon, local time, for Casablanca, Morocco:

The actual temperature (in degrees Celsius)
The forecasted temperature (in degrees Celsius) for the following day at noon
Here is an example of what the the resulting weather report should look like:

![image](https://github.com/prateekrana24/ETL_Historical_Weather_Forecast/assets/88931114/a218a176-277d-47d7-955e-d2a0f10029da)
