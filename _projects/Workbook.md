Bigfoot Sightings Visualizations

Introduction
This assignment involves creating two visualizations using Python, Altair, and Vega-Lite based on the BFRO dataset. The dataset contains detailed information about Bigfoot sightings, including location, date, classification, and environmental conditions. The goal is to uncover patterns in geographical distribution and temporal trends of sightings. Both visualizations include interactivity beyond basic pan/zoom functionality.

Dataset
The dataset used for this assignment is publicly available at the following URL:
https://raw.githubusercontent.com/UIUC-iSchool-DataViz/is445_data/main/bfro_reports_fall2022.csv

Visualization 1: Geographic Heatmap of Bigfoot Sightings
Description
This visualization shows the density of Bigfoot sightings across the United States. Each point represents a sighting, with its size and color encoding the density of sightings in that area.

Design Choices
Encoding Types:

Longitude/Latitude: Used to plot sightings geographically.

Size: Represents the number of sightings in a given location.

Color: A sequential yellow-to-red color scheme indicates sighting density, making it easy to identify hotspots.

Interactivity:

Tooltips display the state and sighting count when hovering over a point.

A dropdown filter allows users to view sightings by state.

Data Transformation
The data was grouped by state, latitude, and longitude to calculate the number of sightings at each location. This aggregation enabled plotting density effectively.

Output
This heatmap highlights hotspots like the Pacific Northwest, known for its Bigfoot lore. The interactivity allows users to explore specific states or regions.



Visualization 2: Temporal Trends in Bigfoot Sightings
Description
This visualization examines how Bigfoot sightings have changed over time. It aggregates sightings by year and separates them by classification (e.g., Class A or Class B).

Design Choices
Encoding Types:

X-axis: Year (temporal encoding).

Y-axis: Number of sightings per year (quantitative encoding).

Color: Different classifications are represented with distinct colors for clarity.

Interactivity:

An interactive legend allows users to toggle visibility for specific classifications.

Tooltips display exact counts for each year and classification.

Data Transformation
The date column was converted to datetime format, and the year was extracted. Data was then grouped by year and classification type to calculate annual counts.

Output
The line chart reveals a peak in Bigfoot reports during the late 1990s and early 2000s. The interactive legend enables users to focus on specific classifications, making it easier to analyze trends.


Discussion of Interactivity
Heatmap:

Tooltips provide detailed information about each state's sighting count.

The dropdown filter allows users to explore specific states or regions interactively.

Line Chart:

The interactive legend lets users toggle visibility for specific classifications, reducing clutter when analyzing trends.

Tooltips display exact counts for each year and classification, offering precise insights.

