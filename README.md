# AirPollutionFinalProject
##Notebooks in this repository
There are several ipython notebooks in this repository. These are designed to break up the individual sections of the project into smaller, self-contained processes. To follow the project process, the optimal order to view these files is:
1. BACKGROUND FILE
2. DataCollection&Cleaning.ipynb
3. ExplotatoryDataAnalysis.ipynb
4. PredictiveLinearModeling.ipynb
5. UnsupervisedAnalysis.ipynb
6. SupervisedAnalysis.ipynb

Each section contains the following information.

**DataCollection&Cleaning.ipynb**
This notebook contains the details of data collection and scraping. All files used in this process are either accessed directly from their links within the notebook or contain in the dropbox repository found at: https://www.dropbox.com/sh/cd95rdgrbm9cpz7/AAAG9758zR1tUMvGsxKtIJzXa?dl=0.

**ExploratoryDataAnalysis.ipynb**
This notebook contains the basic visualizations of the data and simple bivariate analyses.

**PredictiveLinearModeling.ipynb**
This notebook works to build predictive models of the individual pollutants based on demographic and environmental variables. Analysis was validated using cities in France.

**UnsupervisedAnalysis.ipynb**
This notebook works to generate particular clusters of urban areas given their pollutant profiles. Furthermore, it looks at differences in environmental and demographic variables between the clusters.

**SupervisedAnalysis.ipynb**
This notebook seeks to create classifiers to predict which type of pollutant profile a city has given their environmental and demographic characteristics. Analysis was validated using cities in France.

##Data Files in this Repository
There are several files in this repository beyond the ipython notebooks. There are 11 datafiles:<br>
1. FranceMonthDat.csv - Monthly dataset for French cities<br>
2. FranceSeasonDat.csv - Seasonal dataset for French cities<br>
3. FranceYearDat.csv - Yearly dataset for French cities<br>
4. MonthDat.csv - Original monthly dataset for US cities (weather from EPA site)<br>
5. MonthDat2.csv - Updated monthly dataset for US cities (weather from NOAA)<br>
6. SeasonDat.csv - Original seasonal dataset for US cities (weather from EPA site)<br>
7. SeasonDat2.csv - Updated monthly dataset for US cities (weather from NOAA)<br>
8. YearDat.csv - Original yearly dataset for US cities (weather from EPA site)<br>
9. YearDat2.csv - Updated yearly dataset for US cities (weather from NOAA)<br>
10. us_transit_to_tableau.csv - A dataset that was used in tableau to generate a map of transit style across the US<br>
11. dfClusters_kMeans.csv - A file indicating which cluster each US city fell in<br>

##Other files
Beyond these files, there are several image files used throughout notebooks

