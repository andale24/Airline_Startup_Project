![image](https://assets.gulfstream.aero/thedotcom/images/aircraft/g650er/d_g650ER_a_mkt_00186_v02r01_web.jpg)

# Conquer the Sky: How do We Lift Off?

**Authors**: John Baumgartner, Mytreyi Abburu, Andreas Budhi


## Business Problem

 Our company is planning on expanding into the airplane industry. Our stakeholder, the head of the newly created aviation division, is eager to start spearheading this department. But where do we start? We come in to assess the risk of each airplane manufacturer and the type of airplane they make that will present the least risk for our first airplane. We did outside research to see which airplane manufacturers are the top 4 that we can pick. We then analyze these manufacturers and find which presents the least number of accidents and incidents, along with the number of fatal injuries in the past 20 years. Why are these metrics vital for us to consider? As a new company, we want to establish a firm trust with our customers that we will provide the best way for you to travel to your destination.


## Data Understanding

We were using dataset 'AviationData.csv' from the National Transportation Safety Board.  The data includes accident and incident data from 1962 to 2023 in the United States and beyond.

In this data, it contains 88889 entries with a total of 31 columns. 


## Data Analysis

Through an outside resource, we determined that the best way to start was through reputation. Hence, we decided to restrict our exploration to the top 4 airplane manufacturers, and they are Beechcraft, Airbus, Boeing, and Bombardier.

We first added a new column 'Year' to better filter according to year. We then filtered the data to only include accidents after the year 2002 and that occurred in the United States only. 

We cleaned the 'Make' column of our data so that we could see the actual result of our top 4 manufacturers. To do this, we did a manual scanning of each misspelling and other varieties to describe value entry for the top 4 airplane manufacturers. We then set them to the same entry for each of the manufacturers.

In dealing with missing data, we determined that the count for the overall data justified our decision delete the missing data and based our analysis on the remaining data points.

Final dataset N = 2688



### Total Number of Accidents/Incidents for each of the Top 4 Airplane Manufacturers
![graph1](./Image/numberofaccidentsVSmanufacturers.png)

Airbus and Bombardier had the least amount of Accidents/Incidents in the United States.


### Total Number of Fatal Injuries for each of the Top 4 Airplane Manufacturers
![graph2](./Image/manufacturersVSfatalinjuries.png)

We went further to take into account number of Total Fatal Injuries for the top 4 airplane manufacturers in the past 20 years. The graph shows that Airbus and Boeing had the least amount of Total Fatal Injuries.


### Total Number of Injuries for each of the Top 4 Airplane Manufacturers
![graph3](./Image/manufacturersVSinjuries.png)

In regards to Total Injuries, which does not include fatalities, Airbus and Bombardier are responsible for the least amount. 


### Total Fatal Injuries in the past 20 years by year and for each top 4 Manufacturers
![graph4](./Image/fatalinjuryVSyearsmanufacturers.png)

In comparing these graphs, we see that Airbus has been consistent in the past 20 years in having the least amount of Fatal Injuries


### A Trendline View of Total Fatal Injuries in the past 20 years for each top 4 manufacturers
![graph5](./Image/FatalInjuriesTrendline.png)

Here is another view of the Number of Fatal Injuries for each of the top 4 manufacturers with a trendline.


### Total Number of Fatal Injuries for different Types of Engine for each of the Top 4 Airplane Manufacturers
![graph6](./Image/engineVSfatalinjury.png)

This graph tells us that Turbo Shaft and Turbo Jet engine had the least amount of Fatal Injuries.


## Conclusion

After conducting data analysis, we recommend choosing Airbus manufactured airplanes since they have been responsible for only 1% of the fatalities out of the top 4 airplane manufacturers. Since we recommend Airbus, we also recommend to start with commercial airlines. Finally, we also recommend Turbo Jet engine type airplanes since our data analysis indicates that Airbus manufactured Turbo Jet airplanes are responsible for 0 fatal injuries.


## Further Investigation

- Explore and research different Airbus Turbo Jet airplanes, specifically A320ceo and A350F.
- Compare data with total domestic flights.
- Explore and research Bombardier as another possible option.


## Additional Resources

- <p><a href="https://www.phl.org/newsroom/911-security-impact">A Look at How Airport Security has Evolved Post 9-11</a></p>
- <p><a href="https://www.investopedia.com/ask/answers/050415/what-companies-are-major-players-airline-supply-business.asp#:~:text=Large%20Passenger%20Airplane%20Manufacturers,business%20for%20large%20commercial%20jets">Who are the Major Airplane Manufacturing Companies?</a></p>
- <p><a href="https://pilotinstitute.com/airbus-vs-boeing/">Airbus vs Boeing</a></p>
- <p><a href="https://www.aviationsafetymagazine.com/features/the-real-risks-of-engine-failures/">The Real Risks of Engine Failures</a></p>
- <p><a href="https://www.airpowerinc.com/types-of-aircraft-engines">Types of Aircraft Engines</a></p>


## For More Information

Please visit our full analysis in our [Jupyter Notebook](./index.ipynb), [Tableau Dashboard](https://public.tableau.com/app/profile/john.baumgartner/viz/AirlineSafetyReport_16963506541880/IncidentsandFatalitiesoftheFourMajorAirplaneManufacturers?publish=yes), or [Slide Presentation](./Aviation%20Accident%20Analysis.pdf).

For more questions, please feel free to reach us: **John Baumgartner | jtbpilgrim@gmail.com, Mytreyi Abburu | abburumk@gmail.com, Andreas Budhi | ab41571@gmail.com.**


## Repository Structure

You are currently in the README.md file. The 'index.ipynb' file contains the jupyter notebook of the explaratory analysis of the given data that provides step-by-step guide to how we came to our conclusion. 'Images' file contains the images used in this file. The images were taken from the internet.

```
├── Data                             <- Data file used in this project
├── Image                            <- Images and Graphs used in this project obtained from external and internal source
├── .gitignore                       <- Contains list of files to be ignored from GitHub
├── Aviation Accident Analysis.pdf   <- Slide Presentation of the project
├── README.md                        <- Contains README file to be reviewed    
└── index.ipynb                      <- Jupyter notebook of the project containing codes and analysis
```
