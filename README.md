# USA-Covid-data-visualisation

## Goal
The goal of the project is to construct an application to explore data relating to the COVID-19 pandemic. The data set we will use is a public dataset obtained from the New York Times. The application will read in data from a file “covid.csv”,
render it, and allow the user to interact with it. The data will take the following format (comma separated values):  
date, administrative area, county, geo identifier, cases, country  
  
For example:  
21/01/2020, Snohomish, Washington, 53061, 1, United States  
  
Each entry appears on a new line. Varying size datasets will be available from links on blackboard, and the ability to deal with these will depend on the efficiency of your program. You may make use of other datasets to add additional data such as vaccinations, or to map location names to maps. You may also pull in real time data such as daily updates or twitter posts.  
- Date - Date in DD/MM/YYYY format  
- Administrative area – string indicating the area within the county  
- County – string indicating the area within the country  
- Geo identifier – a string representing the geographic location in a format for that country (may be blank)  
- Cases – number of cases reported that day  
- Country – string indicating the country    
Fields are not expected to be empty, but it is best to program defensively.  
  
2. Structure  
The program will contain the following components:  
- code to read in the data from a file and place it in classes.  
  - Processing provides both loadBytes and loadStrings commands  
  - A simple (although not particularly efficient) solution would be to define a DataPoint class which represents a single day for a given area. There would be one instance of the class for each entry in the input file.  
  - You may wish to store the data in a format which is more efficient to access.  
  
- code to select a subset of this data.  
  - Not all the data will be shown on the screen at one time, and so a set of queries must be defined in your code. At a minimum, the following queries should be implemented:  
    - Cases within an area over time
    - The areas with the biggest changes in cases over some time period.
    - Browsing all the areas of a country.
  
- code to draw the data to the screen.  
  - The results of each query will need to drawn on the screen.
  - You are encouraged to use graphical representations where appropriate (eg. the data could be on a barchart, a map, or more complex visualisations such as treemaps or heatmaps).  
  
- code to handle user commands.  
  - Selecting what data is to be displayed (the query), the area or county name, date range, etc.  
  
- code to put everything together  
  - You are advised to have an outline of this as early as possible (first week of project).   
