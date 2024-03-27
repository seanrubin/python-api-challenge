# Part 1: WeatherPy
In this deliverable, you'll create a Python script to visualize the weather of over 500 cities of varying distances from the equator. You'll use the citipy Python libraryLinks to an external site., the OpenWeatherMap APILinks to an external site., and your problem-solving skills to create a representative model of weather across cities.

For this part, you'll use the WeatherPy.ipynb Jupyter notebook provided in the starter code ZIP file. The starter code will guide you through the process of using your Python coding skills to develop a solution to address the required functionalities.

To get started, the code required to generate random geographic coordinates and the nearest city to each latitude and longitude combination is provided.

# Requirement 1: Create Plots to Showcase the Relationship Between Weather Variables and Latitude
To fulfill the first requirement, you'll use the OpenWeatherMap API to retrieve weather data from the cities list generated in the starter code. Next, you'll create a series of scatter plots to showcase the following relationships:

Latitude vs. Temperature
![image](https://github.com/seanrubin/python-api-challenge/assets/31460184/8b73df17-33c4-43ea-9758-23420129654f)

Latitude vs. Humidity
![image](https://github.com/seanrubin/python-api-challenge/assets/31460184/143232c5-891f-46a9-988b-92df6e3e3c08)

Latitude vs. Cloudiness
![image](https://github.com/seanrubin/python-api-challenge/assets/31460184/cff48e2e-755e-4fe3-8c54-c0d681b2ffcc)

Latitude vs. Wind Speed
![image](https://github.com/seanrubin/python-api-challenge/assets/31460184/ef9e87d2-51c6-40ff-8dd3-a2f8f144ebc5)

# Requirement 2: Compute Linear Regression for Each Relationship
To fulfill the second requirement, compute the linear regression for each relationship. Separate the plots into Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude). You may find it helpful to define a function in order to create the linear regression plots.

Next, create a series of scatter plots. Be sure to include the linear regression line, the model's formula, and the r values as you can see in the following image

You should create the following plots:

Northern Hemisphere: Temperature vs. Latitude
![image](https://github.com/seanrubin/python-api-challenge/assets/31460184/1b67160b-83c9-46d4-adee-379ef93d3ad7)

Southern Hemisphere: Temperature vs. Latitude
![image](https://github.com/seanrubin/python-api-challenge/assets/31460184/188f0974-92bc-4156-aed9-1a7d897dc4e5)

Northern Hemisphere: Humidity vs. Latitude
![image](https://github.com/seanrubin/python-api-challenge/assets/31460184/a928c10b-3be1-485d-b431-726c7bd4502c)

Southern Hemisphere: Humidity vs. Latitude
![image](https://github.com/seanrubin/python-api-challenge/assets/31460184/a28dafa5-5cab-4e83-b0a4-b5eacbe58263)

Northern Hemisphere: Cloudiness vs. Latitude
![image](https://github.com/seanrubin/python-api-challenge/assets/31460184/fa3d1d9e-6a12-4536-bd70-4bf66c9a8e1e)

Southern Hemisphere: Cloudiness vs. Latitude
![image](https://github.com/seanrubin/python-api-challenge/assets/31460184/7d4aa91f-7fe6-4985-b806-e8433acd216d)

Northern Hemisphere: Wind Speed vs. Latitude
![image](https://github.com/seanrubin/python-api-challenge/assets/31460184/bd608923-533c-41ea-bd8c-02f2fdd0b1d3)

Southern Hemisphere: Wind Speed vs. Latitude
![image](https://github.com/seanrubin/python-api-challenge/assets/31460184/7b5dd15f-6702-485e-a485-d56d2dd9c044)


# Part 2: VacationPy
In this deliverable, you'll use your weather data skills to plan future vacations. Also, you'll use Jupyter notebooks, the geoViews Python library, and the Geoapify API.

The code needed to import the required libraries and load the CSV file with the weather and coordinates data for each city created in Part 1 is provided to help you get started.

Your main tasks will be to use the Geoapify API and the geoViews Python library and employ your Python skills to create map visualizations.

To succeed on this deliverable of the assignment, open the VacationPy.ipynb starter code and complete the following steps:

Create a map that displays a point for every city in the city_data_df DataFrame as shown in the following image. The size of the point should be the humidity in each city.

Humidity map
![image](https://github.com/seanrubin/python-api-challenge/assets/31460184/be0037d5-9281-43c0-8d46-293848203bd6)

Narrow down the city_data_df DataFrame to find your ideal weather condition. For example:

A max temperature lower than 27 degrees but higher than 21

Wind speed less than 4.5 m/s

Zero cloudiness

Create a new DataFrame called hotel_df to store the city, country, coordinates, and humidity.

For each city, use the Geoapify API to find the first hotel located within 10,000 meters of your coordinates.

Add the hotel name and the country as additional information in the hover message for each city on the map as in the following image:
![image](https://github.com/seanrubin/python-api-challenge/assets/31460184/db8a06a0-0198-4290-9b28-d59ed6379078)

