# AirPollutionFinalProject
##Background and Motivation
The World Health Organization reported that in 2012 about 7 million people died as a result of air pollution exposure, a finding that was more than double previous estimates.  According to the WHO, this finding “confirms that air pollution is now the world’s largest single environmental health risk.”  Air pollution can lead to a variety of potentially fatal conditions such as heart disease, stroke, COPD, and lung cancer.  Thus it is critical that more research on air pollution causes and interventions to reduce such pollution be done.
 
As students at the Harvard T.H. Chan School of Public Health, we want to conduct some research into air pollution in the USA as well as on some of the determinants of such pollution such as weather, commuting, and population density given the severity of this public health issue.  By understanding the pollutant profiles of various cities, more targeted and effective interventions for reducing pollution on a by-pollutant-type basis could then be proposed and implemented.  Linking these specific profiles to certain determinants would also aid in the creation of powerful air pollution reduction policies.  These various analyses could be useful for developing legislation across the USA.  Additionally, we could predict the pollutant profiles of cities in the third world, where such measuring of pollutants is not available, based on weather, population, etc.  Such prediction would allow for better formulation of air pollution reduction policies for those cities.
Initial Questions:<br>
·       Are there certain pollutant profiles that characterize groups of US cities?<br>
·       What is the distribution of pollutants (air particulate matter, gas levels, etc.) within these clusters?<br>
·       What are the determinants (weather, demographics, transportation, etc.) of these pollutant profiles?<br>
·       Can we use data on weather, demographics, transportation, etc. to predict a city’s pollutant profiles?<br>
·       Can specific policy recommendations be made based on a city’s pollutant profile?<br.

##Notebooks in this repository
There are several ipython notebooks in this repository. These are designed to break up the individual sections of the project into smaller, self-contained processes. To follow the project process, the optimal order to view these files is:<br>
1. DataCollection&Cleaning.ipynb<br>
2. ExplotatoryDataAnalysis.ipynb<br>
3. PredictiveLinearModeling.ipynb<br>
4. UnsupervisedAnalysis.ipynb<br>
5. SupervisedAnalysis.ipynb<br>

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

