# project_crime_vs_density_green_spaces
## Project title
### City and crime: how green spaces and density influence criminality in Berlin

## Motivation
Where crimes happen? How distribution of green spaces influence criminality? How density influence criminality? What is the correlation between size, type and structure of green spaces and numbers of crimes? How could neighbourhoods be clustered based on criminality, green spaces and density?
To answer those questions the case study object was chosen: the city of Berlin divided into 143 subdistricts (neighbourhoods). For each district it was analysed, what is the crime ratio and how it could be correlated with the spatial structure: density and green spaces. 
The author, who possesses a robust background in natural sciences and landscape design, selected this research topic based on personal interests as she believes, the way we design city matters in many different areas of our life. 

## Dataset Information 
To conduct the project the following data was collected and analysed:
* Districts and neighbourhoods - LOR classification
  (via WFS from Geoportal Berlin (spatial analysis) and numerical data)
https://daten.berlin.de/datensaetze/lebensweltlich-orientierte-r%C3%A4ume-lor-planungsr%C3%A4ume-01012021-wfs
https://fbinter.stadt-berlin.de/fb/gisbroker.do;jsessionid=D2DD12D2AF97F589C307BD557890DBD5?cmd=alphaDataDownload   
* Criminality in Berlin (2013-2022)
https://daten.berlin.de/datensaetze/kriminalit%C3%A4tsatlas-berlin
* Green spaces: parks and playgrounds (via WFS from Geoportal Berlin)
https://fbinter.stadt-berlin.de/fb?loginkey=showMap&mapId=gris_oeffgruen@senstadt 
* Green spaces: forests (via WFS from Geoportal Berlin)
https://fbinter.stadt-berlin.de/fb?loginkey=showMap&mapId=k06_02_freifl@senstadt
* Green spaces: cemetries (via WFS from Geoportal Berlin)
https://fbinter.stadt-berlin.de/fb/index.jsp?loginkey=showMap&mapId=friedh@senstadt
* Green spaces: allotment gardens (via WFS from Geoportal Berlin)
https://fbinter.stadt-berlin.de/fb/index.jsp?loginkey=showMap&mapId=kleing@senstadt
* Density (2013-2020)
https://web.statistik-berlin-brandenburg.de/instantatlas/interaktivekarten/kommunalatlas/atlas.html
* Density (2021)
https://web.statistik-berlin-brandenburg.de/instantatlas/interaktivekarten/kommunalatlas2021/atlas.html
* Crime index:
https://www.numbeo.com/crime/region_rankings_current.jsp?region=150   


## Project description and how to use 
### Goals, methodology and conclusions
The goal of the project was to investigate whether there is a correlation between criminal activity from 2013 to 2021 and population density and green space availability in the city. The case study focused on the city of Berlin, which is divided into 143 subdistricts (known as LOR in Berlin).

Criminal activity was measured using the crime ratio, defined as the number of reported crimes per capita within a subdistrict. In addition to total crime cases, specific categories such as robberies, drug offenses, and graffiti were analyzed. The distribution of crimes within the city was examined in relation to two factors: the distribution of green spaces and population density.

Multiple analyses were conducted using Python and QGIS to assess how the distribution of different types of crime varied. Spatial data on green spaces was collected and analyzed numerically using Python and spatially and numerically using QGIS.

It was concluded that high population density has a direct impact on the overall crime ratio and the number of robberies. A high green space ratio, defined as the percentage of subdistrict area covered by green spaces, was found to decrease the crime ratio. However, there were exceptions, as not only the green space ratio but also the distribution and type of green areas proved to be important factors. Additionally, it was observed that for certain types of crime, such as graffiti and drug offenses, the distribution differed slightly, with some crimes occurring in less populated areas with higher green space ratios, where less social control was evident. 

### Steps to conclude the project:
1. Creating a project board on Trello
- https://trello.com/b/qayH4Fo2/final-projectkatarzyna
2. Notebook file: 1_criminality:
- Importing, cleaning and preparing the dataset with criminality in the last 9 years for Berlin.
3.	Notebook file: 2_density_lor:
-	Combining datasets with population, and subdistricts of Berlin. 
4.	Gathering spatial data to green areas in QGIS via WFS:
-	Infos to 5 types of green spaces: cemeteries, allotment gardens, parks, playgrounds, forests. 
-	Spatial joining those data with subdistricts (lor).
-	Output: datasets with all 5 green spaces types: playgrounds_lor_tab.xlsx, parks_lor_tab.xlsx, forests_lor_tab.xlsx, cemetries_lor_tab.xlsx, allotment_lor_tab.xlsx.
-	Output: green_spaces_summary.xlsx
5. Notebook file: 4_crimi_2021:
-	Combining info to criminality, green spaces, density and population. 
6.	Notebook file: 5_clustering
-	Creating clusters for subdistricts. 
7.	Notebook file: 6_formatting_for_qgis
8.	Notebook file: 7_web_scraping.
9.	Combining numerical and spatial data in QGIS and creating visualisations there.
10.	The further analysis and visualisations were conducted in Tableau:
- https://public.tableau.com/views/crime_vs_density_final/robb_den_3cases?:language=de-DE&publish=yes&:sid=&:display_count=n&:origin=viz_share_link
11.	Presentation is attached in the documentation. 

## Tech/framework used
Python: Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn(Sklearn), BeautifulSoup4.
Jupyter Notebook
Anaconda
QGIS
Tableau
GitHub
GitBash
Trello

## Features
Combining the data analytics techniques to the city planning and conducting spatial analysis using Python and QGIS Software. 

## Installation
Used version Python 3.11.5


You would be needing multiple libraries such as Math, Numpy, Pandas and Seabon for basic operations and many pre-processing and ML Model libraries.
- pip install [Library_Name] 

  
