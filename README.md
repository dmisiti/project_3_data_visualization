For our third project, we decided to take a look at the attendance rates for kids between the school years k-12 by their school district
and we also included the summarized data as a whole state. Our goal was to see if there were any interesting trends with the students in Connecticut and their attendance rates as well as how some external factors come into play when looking at the attendance for students. 

To interact with our projects, we have two interactive dashboards that are run through our code. The first code file is called graphing_with_dash.ipynb. This is a code where when it is run, it shows a dashboard of a bar graph and a line graph. These graphs both show data using our dataset and there are three different topics to choose from where the graphs are both linked and change depending on the topic. The second code file is geopandas/pydeck_map. It shows a map of all students in Connecticut and it has layers that show students with high needs and students without high needs so the end user is able to run the code and toggle between the layers.


When it came time to use a database, we chose to use PostgresSQL as our database of choice. We thought that using Postgres SQL to hold all of our data was a good idea because
with this we are able to hold a base dataset of data in postgres and then we are able to make changes/clean anything we need to in jupyter notebooks so that the datasets were
ready to use for our visuals. The Postgres SQL database was good because if we ever messed up, we could get go back and pull our base database from Postgres and start over again. 

Being ethical with data is something that is being brought up a lot in the news and is very important in terms of protect people's information. In our project, we made sure to be very ethical with the data that we are presenting. We looked through each of the datasets that we had to make sure that there was no private information in them such as Date of birth or student's full names. We intend to use the data that we have to paint a broad picture of different students groups from each district and compare them to one another. None of what we are trying to do is to display or even analyze sensitive information espically if they don't want it out there. We have made sure of this and believe that our dataset achieves this. 



References: 

Data sources:
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

