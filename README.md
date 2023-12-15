# Unmasking the Epidemic: Analyzing the Complex Factors Behind Gun Violence in the United States 
### By Tanay Kumar Sayala, Ben George Samuel, Ravi Varma Pakalapati 

## Section 1: Why and How 
In just the past decade, the United States has witnessed a disturbing increase in the frequency of acts of 
gun violence. Sadly, one group that gets severely affected by this is schoolchildren. Any sort of traumatic 
experience can have long-lasting negative psychological effects on a child’s developing brain; there 
doesn’t have to be a death for an experience to be categorically traumatic for a child. Many Band-Aid 
solutions have arisen as a result of this severe uptick in incidents, however, none aim for the head of the 
beast for various reasons. Our project, outlined below, aims to thoroughly analyze data collected in the 
K-12 School Shooting Database (k12ssdb.org). The data collected here details all shootings at schools. 
“All shootings at schools includes when a gun is brandished, is fired, or a bullet hits school property for 
any reason, regardless of the number of victims, time, or day of the week… (and the collected data also 
includes) gang shootings, domestic violence, shootings at sports games and afterhours school events, 
suicides, fights that escalate into shootings, and accidents” (k12ssdb.org).

We intend to visualize the distribution of gun violence across the US over time. The K12SSD has been 
kept up to date, and provides data for every recorded instance of gun violence in schools from 1966 to 
the present day. The visualizations will show how gun violence has been present in the various regions in 
the US, along with each region’s poverty rate. We would like to see if there is any correlation present. 
Above all, we’d like to show as much regional data as possible, specifically county specific information, so 
that we can have an effective drill-down. 

 
## Section 2: Design 
We have designed 3 sections of visualizations, detailed below: 

Fig 1, Time Series Line Graph 
This visualizes the total number of incidents that occurred from 1966 to 2023. Each point on the line refers to a specific 
year, and shows the trend of gun violence throughout the years. This visualization is purely meant to show the alarming 
increase in incidents in recent years. 

Fig 2, Interactive Choropleth Map 
This visualizes the data related to school shootings, poverty percentage, and educational information at the state and county 
levels in the United States. The map is implemented using an SVG container with features like zooming and tooltip 
interactions. The map is dynamically updated based on selected filters, including years and school types. The data, consisting 
of GeoJSON information for U.S. states and a CSV file with details on school shootings and poverty percentages, is loaded 
asynchronously. The choropleth colors represent the number of shootings in each state, with tooltips displaying additional 
information such as poverty percentage. The code includes functions for handling mouse events, semantic zooming, and 
double-clicking to zoom out. Zooming in shows county-level information as opposed to state information while zoomed out. 
Filters, including a year range slider and a dropdown for school types, enable users to explore the data interactively. The 
map is initially populated with default filters on page load, and users can adjust filters to explore specific subsets of the data. 

Fig 3, Bar Charts 
The final section of the webpage has 4 bar chart visualizations in separate SVG containers, showing the types of school 
where the shooting incidents happened (fig 3A), the top 5 states where the incidents occurred (fig 3B), incidents distributed 
across the months when they occurred (fig 3C), and the 5 cities with the most incidents in a selected region (fig 3D). All four 
of these graphs show data for the year range selected by the user. Clicking on a corresponding state’s bar in the top 5 states 
graph (fig 3B) allows you to update the region in which the cities bar graph (fig 3D) pulls its data from. These charts also 
incorporate tooltips for additional, detailed information, creating an immersive user interface. 


## Section 3: Discussion 
We were able to effectively visualize how gun violence is distributed across the country, and we can 
begin to draw conclusions regarding shooting counts and socioeconomic status. Due to time constraints 
and a lack of data availability, we had to pare down the scope of the project significantly. The original 
project proposal included filtering for a variety of different factors that may have had an impact on gun 
violence. These included resources available for mental health, political lean, and racial demographics. 
While these filters would not be difficult to implement, sourcing accurate data, for example with mental 
health statistics, proved to be an issue. We also did not want to draw any sort of conclusions that have 
the potential to harm or offend any user, so for the scope of this project, we chose not to include the 
other two potentially polarizing filters. However, given more time, we would implement these filters as 
they provide valuable insights on potential correlations. Finding any additional correlations with these 
extra filters would allow us to actually o formulate targeted interventions and policies to make schools 
safer for all students and educators. 
A) B) C)
D)
