# School Attendances Rates in Connecticut, 2019-2022

## Topic
Data was collected for public school attendance in Connecticut over the course of three school years from 2019-2022. In this project, analysis was performed to consider any trends or insights in attendance rates between different student groups and different school districts across connecticut. Questions considered include:

1. How does the attendance rate of each student group compare to the overall attendance rate of students in Connecticut over the course of these three years?
2. With the national average attendance rate today being approximately 90%, how does the data from Connecticut compare to this threshold?
3. How did attendance rates changes from year to year? Were their any observable differences for any particular student groups when the pandemic began in 2020?
4. In a given school distract, does the population of higher-need students correlate to a higher or lower attendance rate?

## Dataset
The primary dataset for this project can be found here. ​​(Refer to the "images" folder for a screenshot of the metadata.) This dataset includes the attendance rates for Connecticut public school students in grades PK-12. The data is grouped by student category as well as by school district. The data is from three school years: 2019-20, 2020-21, and 2021-22. The student groups that are in our dataset are listed below:

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

Several new libraries were used in the process of this data analysis:
- [Dash](https://dash.plotly.com/tutorial)
- [Folium](https://realpython.com/python-folium-web-maps-from-data/)
- [Pydeck](https://deckgl.readthedocs.io/en/latest/layer.html)
- [Geopandas](https://geopandas.org/en/stable/docs/user_guide/geocoding.html)
-[Sharpely](https://geopandas.org/en/stable/gallery/create_geopandas_from_pandas.html)
- [Contextily](https://pypi.org/project/contextily/)

## Project Inspiration & Initial Design

Data Visualization #1 – Mapping attendance rates by school district and displaying a pop up on each with attendance statistics

Data Visualization #2 – Bar graph displaying attendance rates by student category compared to the average attendance rate for a student in America

Data Visualization #3 – 3D map of attendance rates, with the higher the bar showing lower attendance rates

Data Visualization #4 – Line graph showing changes in attendance rates over the three years of data collection in Connecticut, with a reference line on the graph showing when the covid pandemic began

(Refer to the "images" folder for screenshots of visualization inspiration.)

## Ethical Considerations
Being ethical with data is something that is being brought up a lot in the news and is very important in terms of protect people's information. In our project, we made sure to be very ethical with the data that we are presenting. We looked through each of the datasets that we had to make sure that there was no private information in them such as Date of birth or student's full names. We intend to use the data that we have to paint a broad picture of different students groups from each district and compare them to one another. None of what we are trying to do is to display or even analyze sensitive information espically if they don't want it out there. We have made sure of this and believe that our dataset achieves this.

## Repository Structure
The end-product of our analyis was two interactive visualizations:
- Data Visualization Dashboard – CT School Attendance Rates from 2019-2022
- Interactive Map – CT School Attendance Rates by District during the 2021-2022 School Year

The Data Visualization Dashboard can be accessed via the `graphing_with_dash.ipynb` notebook.
- This notebook contains the coding script for all bar graphs and line graphs that were created, ultimately displaying them on one singular dashboard that provides a dropdown box to toggle between different graphs based on different categories of students.

The Interactive Map can be accessed via the `folium_map.ipynb` notebook.
- This map displays a dot for each school district in Connecticut, with a toggle between three different layers: All Students, Students with High Needs, and Students without High Needs. Dot size correlates to student population in the district, and dot color correlates to attendance rates (green = higher attendance rates, red = lower attendance rates). Each dot displays the district name and attendance rate when hovered over.

Other files in this repository were used to reach our end visualizations:
- `postgreSQL_imports.ipynb`: This file was used for importing the two initial dataset CSVs, pulled in from PostgreSQL. (The CSVs are found in the "resources" folder under `attendance_table.csv` and `locations_table.csv`.)
- `data_cleaning.ipynb`: This file was used for cleaning and merging the two imported CSVs into one final CSV to be used for our analysis
- `geopandas_pydeck_map.ipynb` and `project3_eda_notes`: This file was used for exploratory data analysis and initial mapping creations before creating the final mapping product in Folium.

The presentation slides for all materials, including screenshots of all graphs and map displays, can be found in the `project3_slides.pdf` file.

## Conclusions
Attendance Rates by Level of Need
- The attendance rates of students with high needs were consistently lower than that of students without high needs. This disparity especially increased following the onset of the covid-19 pandemic, as seen in the 2020-21 and 2021-22 school year data.

Attendance Rates by Category of Need
- Students with all categories of need fall at our below the average attendance rate for students in Connecticut over the course of the three years of this data.
- Students experiencing homelessness showed the lowest attendance rates of all the different categories ov need, and especially dropped with the onset of the covid-19 pandemic, as seen in the 2020-21 and 2021-22 school year data.

Attendance Rates by Race/Ethnicity
- The attendance rates of students of Black/African American students and Hispanic/Latino students were consistently lower than that White students and students of all others races. This disparity especially increased following the onset of the covid-19 pandemic, as seen in the 2020-21 and 2021-22 school year data.

Mapping Attendance Rates by District
- Districts that have more students with high needs also have a lower rate of school attendance.
- District size also often correlates with attendance; the greater the student count, the lower the rate of attendance.

## Future Considerations
It would be interesting to explore in the future how the data has progressed in Connecticut schools over the last few years, as well as looking at private school data and comparing to the public school data from this set. It would also be interesting to look further into reasonings behind attendance rates by different categories beyond the context of the covid-19 pandemic. Additionally, on the data visualization side of things, some exploration was done in this project on 3D modeling maps, and it would be interesting in the future to plot the mapping data where population size or attendance rates were represented visually on the z-axis.

## References
Dataset that had the location for each school district: Education Directory | Connecticut Data, data.ct.gov/Education/Education-Directory/9k2y-kqxn/data. Accessed 7 Jan. 2025.

Dataset for attendance rates by district: “State of Connecticut - School Attendance by Student Group and District, 2021-2022.” Catalog, Publisher data.ct.gov, 19 Aug. 2023, catalog.data.gov/dataset/school-attendance-by-student-group-and-district-2021-2022.
