## EDA Project Write-Up

 

#### Abstract

The goal of this project was to analyze New York City’s MTA Transit data, to see which MTA station near New York University has the most exit foot traffic during the Fall Move-In period/start of classes. The results showed that while there was no sharp increase in exit foot traffic during move-in week or the first week of classes, the West 4th-Washington Sq station was consistently the most popular station, with 4-8pm being the busiest time period. The exit traffic on weekdays in 2020 and 2021 are lower compared to the years before the pandemic, when classes were fully in-person.

#### Design

My hypothetical client, the Bonomi Family Admissions Center at NYU, wants me to figure out a way to help incoming freshmen and transfer students navigate to their desired campus destinations (dorm buildings, classrooms, etc.) during the beginning of Fall semester. Adapting to an urban campus as an incoming university freshman or transfer student can be overwhelming. It’s challenging to figure out who to ask, and not every building in the area is a campus building. This project aims to find the best time and location for placing upperclassman volunteers at each of the 4 stations closest to NYU, in proportion to the volume of people exiting the station. 

 #### Data

The dataset from 4 months (mid-Aug to mid-Sept from years 2018-2021) contains 3293897 rows. I narrowed down to the data to focus on turnstile exits at 4 stations: Astor Place, 8th-Street NYU, West 4th St-Washington Sq, and Christopher St-Sheridan Sq. These stations were listed on the NYU website, and combined they represent stops for the following lines: A, B, C, D, E, F, M, N, R, W, 1, and 6. They also connect to popular travel hubs: Grand Central Station, Port Authority, and the La Guardia/JFK/Newark airports. I focused on exits to depict the foot traffic entering onto campus, but this is still an overestimate as not everyone exiting the station is an NYU student.

#### Algorithms

A thorough Exploratory Data Analysis was performed, which included cleaning, aggregating, and visualizing the data. 

 #### Tools

\-    SQLAlchemy to import data from the SQLite database into Python 

\-    Matplotlib and Seaborn for plotting/visualizations

\-    Numpy and Pandas for data manipulation

#### Communication

To compare the timing of move-in and start of Fall classes with the number of exits each day, I plotted 4 time-series graphs (one for each station) with each year as a line. The x-axis was standardized since each year’s data was from the same set of days. To explore the most popular timeframe, I plotted the exit data into stacked bar charts graphs, with each graph representing a different year. Each stacked bar represents the total number of exits from the station within each time period (8am to 12pm, 12pm to 4pm, or 4pm to 8pm. The results were communicated through a final presentation, with the slides and code available in this repository. 
