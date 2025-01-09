# School Attendances Rates in Connecticut, 2019-2022

## Topic
Data was collected for public school attendance in Connecticut over the course of three school years from 2019-2022. In this project, analysis was performed to consider any trends or insights in attendance rates between different student groups and different school districts across connecticut. Questions considered include:

1. How does the attendance rate of each student group compare to the overall attendance rate of students in Connecticut over the course of these three years?
2. With the national average attendance rate today being approximately 90%, how does the data from Connecticut compare to this threshold?
3. How did attendance rates changes from year to year? Were their any observable differences for any particular student groups when the pandemic began in 2020?
4. In a given school distract, does the population of higher-need students correlate to a higher or lower attendance rate?

## Dataset
The primary dataset for this project can be found here. ​​This dataset includes the attendance rates for Connecticut public school students in grades PK-12. The data is grouped by student category as well as by school district. The data is from three school years: 2019-20, 2020-21, and 2021-22. The student groups that are in our dataset are listed below:

Students Grouped by Level of Need
- Students with high needs*
- Students without high needs

Students Grouped by Category of Need
- Students Experiencing Homelessness
- Students With Disabilities
- Free Meal Eligible
- Reduced Price Meal Eligible
- English Learners

Students Grouped by Race/Ethnicity
- Black or African American
- Hispanic/Latino of any race
- White
- All other races

Note: Students with high needs are defined in this study as students who: are English language learners; receive special eduction; and/or qualify for free or reduced lunch.

Additionally, this dataset provides locations and coordinates for schools within each school district, and was eventually merged with the primary dataset to match with Connecticut district names. One school was selected from each district to be used for representative coordinates for each district.

## MetaData
Our metadata is located in our images folder under the name metadata.jpeg.

## Project Inspiration & Initial Design

Data Visualization #1 – Mapping attendance rates by school district and displaying a pop up on each with attendance statistics

Data Visualization #2 – Bar graph displaying attendance rates by student category compared to the average attendance rate for a student in America

Data Visualization #3 – Line graph showing changes in attendance rates over the three years of data collection in Connecticut, with a reference line on the graph showing when the covid pandemic began.

## Ethical Considerations

Being ethical with data is something that is being brought up a lot in the news and is very important in terms of protect people's information. In our project, we made sure to be very ethical with the data that we are presenting. We looked through each of the datasets that we had to make sure that there was no private information in them such as Date of birth or student's full names. We intend to use the data that we have to paint a broad picture of different students groups from each district and compare them to one another. None of what we are trying to do is to display or even analyze sensitive information espically if they don't want it out there. We have made sure of this and believe that our dataset achieves this. 

## Repository Structure

To interact with our projects, we have two interactive dashboards that are run through our code. The first code file is called graphing_with_dash.ipynb. This is a code where when it is run, it shows a dashboard of a bar graph and a line graph. These graphs both show data using our dataset and there are three different topics to choose from where the graphs are both linked and change depending on the topic. The second code file is geopandas/pydeck_map. It shows a map of all students in Connecticut and it has layers that show students with high needs and students without high needs so the end user is able to run the code and toggle between the layers.


## Data sources:

1. Dataset that had the location for each school district:
Education Directory | Connecticut Data, data.ct.gov/Education/Education-Directory/9k2y-kqxn/data. Accessed 7 Jan. 2025.

2. Dataset for attendance rates by district: 
“State of Connecticut - School Attendance by Student Group and District, 2021-2022.” Catalog, Publisher data.ct.gov, 19 Aug. 2023, catalog.data.gov/dataset/school-attendance-by-student-group-and-district-2021-2022.

3. Data for the Cartographic Boundary for the state of connecitcut - US Census Bureau. (2024, April 15). Cartographic boundary files. Census.gov. https://www.census.gov/geographies/mapping-files/time-series/geo/cartographic-boundary.html

4. Documents for how to use Geopandas and converting
'Merging data — GeoPandas 1.0.1+0.g747d66e.dirty documentation. (n.d.). https://geopandas.org/en/stable/docs/user_guide/mergingdata.html'

6. Documents on how to use layers in pydeck library for a geopandas dataset
Layer Overview and Examples — pydeck 0.9.1 documentation. (n.d.). https://deckgl.readthedocs.io/en/latest/layer.html

7. research documents/codes for making a 3D map for a geopandas dataFrame 
https://medium.com/@leodpereda/create-a-beautiful-3d-map-with-pydeck-geopandas-and-pandas-8cd1d73e1ec3

8. 3D plotting — Python Numerical Methods. (n.d.). https://pythonnumericalmethods.studentorg.berkeley.edu/notebooks/chapter12.02-3D-Plotting.html

9. Interactive Mapping using geoPandas
https://geopandas.org/en/stable/docs/user_guide/interactive_mapping.html#


