# Carbon Footprint Calculator

This project is a Carbon Footprint Calculator built using Python and Tkinter for the user interface. It calculates the carbon footprint of a user based on their travel habits, car usage, diet, electricity consumption, and country of residence.

### Disclaimer 
Generally, I like using jupyter notebooks for demonstrating ideas to people, I had intended this to be a teaching notebook for my friends and colleagues. Unfortunately for this project, I found other sources for teaching this information and so, after doing enough of this project to better understand the data, I transitioned towards teaching others with those pre-made (and prettier tools). I will continue to develop this tool for fun, but I add this note for any potential employers who are curious about my decisions

## Table of Contents

- [Usage](#usage)
- [Issues](#issues)
- [Features](#features)
- [Data Sources](#data-sources)
- [Functions](#functions)
- [File Descriptions](#file-descriptions)
- [Contact](#contact)

## Usage

1.  Open a jupyter notebook and run all cells.
2.  A Tkinter window will open, guiding you through a series of questions to gather data about your carbon footprint.
3.  After answering all the questions, the calculator will compute and display your carbon footprint based on the provided data.

## Issues
- There are a lot of issues with this code as I have not had time to do a thorough debugging/data quality verification/full build out of this data. I used this simply to get a better understanding of various data. Over time, I expect to edit this, but if you have specific things you would like to see, feel free to edit it! 

## Features

- **Flight Information**: Calculates emissions based on the type and number of flights taken.
- **Car Usage**: Calculates emissions based on car type, miles driven, and fuel efficiency.
- **Electricity Usage**: Calculates emissions based on annual kWh usage and country-specific energy intensity.
- **Diet**: Calculates emissions based on diet type.
- **Country Specific Data**: Adjusts calculations based on the country of residence to account for different energy mixes and intensities.

## Data Sources

- [Our World in Data](https://ourworldindata.org/)
- [National Center for Biotechnology Information](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4372775/)
- [University of California, Irvine](https://www.physics.uci.edu/~silverma/actions/greenhousereduction.html)
- [World Nuclear Association](https://www.world-nuclear.org/)
- [UK Government](https://www.gov.uk/government/publications/greenhouse-gas-reporting-conversion-factors-2022)
- [Various Articles](see script comments for details)

## Functions

### User Interface

- `openpage(number, page)`: Opens a new page for user input.
- `countPage(thing_to_count, page, delta, number)`: Opens a counting page for numerical inputs.

### Calculations

- `driving(car_type, mileage, miles_per_year, energy_of_country, intensity_of_country)`: Calculates emissions from driving.
- `car_manufacturing(car_type, new)`: Estimates emissions from car manufacturing.
- `food_emission(diet)`: Calculates emissions based on diet.
- `electricity(kwh, energy_of_country, intensity_of_country)`: Calculates emissions from electricity usage.
- `flight_habits(flights_per_year, length, class_type, roundtrip, country, mode)`: Calculates emissions from flight habits.
- `rail(miles_per_year)`: Calculates emissions from rail travel.

## File Descriptions

- `carbon_estimates.ipynb`: Main script containing the Tkinter UI and calculation functions.
- `OurWorldInDataEnergy.csv`: CSV file containing energy data per country.
- `CarbonIntensityWorld.csv`: CSV file containing carbon intensity data per country.
- `per-capita-co2-aviation-adjusted.csv`: CSV file containing average CO2 per capita from aviation data per country.

## Contact

For any questions or feedback, please contact jeffrey.michel.4695@gmail.com.
