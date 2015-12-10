# AirPollutionFinalProject
##Background and Motivation
The World Health Organization reported that in 2012 about 7 million people died as a result of air pollution exposure, a finding that was more than double previous estimates.  According to the WHO, this finding “confirms that air pollution is now the world’s largest single environmental health risk.”  Air pollution can lead to a variety of potentially fatal conditions such as heart disease, stroke, COPD, and lung cancer.  Thus it is critical that more research on air pollution causes and interventions to reduce such pollution be done.
 
As students at the Harvard T.H. Chan School of Public Health, we want to conduct some research into air pollution in the USA as well as on some of the determinants of such pollution such as weather, commuting, and population density given the severity of this public health issue.  By understanding the pollutant profiles of various cities, more targeted and effective interventions for reducing pollution on a by-pollutant-type basis could then be proposed and implemented.  Linking these specific profiles to certain determinants would also aid in the creation of powerful air pollution reduction policies.  These various analyses could be useful for developing legislation across the USA.  Additionally, we could predict the pollutant profiles of cities in the third world, where such measuring of pollutants is not available, based on weather, population, etc.  Such prediction would allow for better formulation of air pollution reduction policies for those cities.
Initial Questions:<br>
<ul>
<li>Are there certain pollutant profiles that characterize groups of US cities?</li>
<li>What is the distribution of pollutants (air particulate matter, gas levels, etc.) within these clusters?</li>
<li>What are the determinants (weather, demographics, transportation, etc.) of these pollutant profiles?</li>
<li>Can we use data on weather, demographics, transportation, etc. to predict a city’s pollutant profiles?</li>
<li>Can specific policy recommendations be made based on a city’s pollutant profile?</li>
</ul>

##Related Work
We were partly inspired by this interesting visualization that shows the relative contribution of different environmental and anthropogenic factors on climate change trends.<br>
http://www.bloomberg.com/graphics/2015-whats-warming-the-world/?utm_source=The+Weekly+Pique&utm_campaign=cf7d4cd5ac-Episode+12%3A+Global+Warming&utm_medium=email&utm_term=0_4627876a86-cf7d4cd5ac-297062977

Another source of inspiration was this interactive map of air quality across all continents:<br>
http://aqicn.org/map/world/

##Key Findings
Based on our analysis, air quality appears to be a composite of many features, some related to human activity and some related to environmental sources. The relative contribution of these two sources seems to vary across pollutants which has implications about how to design effective overall air quality interventions. Using multiple modeling approaches, we find that some pollutant concentrations, such as NO<sub>2</sub> and O<sub>3</sub>, are easier to predict than others. Additionally, US cities can be clustered into distinct pollutant profiles which are differentiated by environmental and demographic factors.<br>
<ul>
<li>Airborne NO<sub>2</sub>, PM2.5, and O<sub>3</sub> of cities can be somewhat predicted based on demographic and weather features, but PM10, CO, and SO<sub>2</sub> are not well described from these characteristics</li>
<li>Prediction models based on US cities do not extend well to French cities</li>
<li>The relative importance of anthropogenic and environmental factors to air pollutant concentrations varies between pollutants</li>
<li>Distinct types of cities exist that can be characterized by their particular pollutant profiles</li>
 <ul><li>These clusters can be differentiated by liquid precipitation, air pressure, temperature, and land area</li></ul>
<li>Differential patterns of missing pollutant data for US cities made imputation of clusters unreliable.</li>
<li>When French cities were clustered with the same method, their pollutant profiles looked reasonably similar to the clustered US pollutant profiles.</li>
</ul>

##Notebooks in this repository<br>
There are several ipython notebooks in this repository. These are designed to break up the individual sections of the project into smaller, self-contained processes. To follow the project process, the optimal order to view these files is:<br>
0. Prologue.ipynb<br>
1. DataCollection&Cleaning.ipynb<br>
2. ExplotatoryDataAnalysis.ipynb<br>
3. PredictiveLinearModeling.ipynb<br>
4. UnsupervisedAnalysis.ipynb<br>
5. UnsupervisedLearning_pt2.ipynb<br>

Each section contains the following information.<br>
[**Prologue.ipynb**](https://github.com/mchaffin17/AirPollutionFinalProject/blob/master/0.Prologue.ipynb)
This notebook contains the information included in this README. This includes background and motivation, initial questions, and guidance on how to navigate the github repo.

[**DataCollection&Cleaning.ipynb**](https://github.com/mchaffin17/AirPollutionFinalProject/blob/master/1.DataCollection%26Cleaning.ipynb)
This notebook contains the details of data collection and scraping. All files used in this process are either accessed directly from their links within the notebook or contained in the dropbox repository found at: https://www.dropbox.com/sh/cd95rdgrbm9cpz7/AAAG9758zR1tUMvGsxKtIJzXa?dl=0.

[**ExploratoryDataAnalysis.ipynb**](https://github.com/mchaffin17/AirPollutionFinalProject/blob/master/2.ExploratoryDataAnalysis.ipynb)
This notebook contains the basic visualizations of the data and simple bivariate analyses.

[**PredictiveLinearModeling.ipynb**](https://github.com/mchaffin17/AirPollutionFinalProject/blob/master/3.PredictiveLinearModeling.ipynb)
This notebook works to build predictive models of the individual pollutants based on demographic and environmental variables. Analysis was validated using cities in France. Additionally, attempts at statistical inference about drivers of particular pollutants using GEE's is found in this notebook.

[**UnsupervisedAnalysis.ipynb**](https://github.com/mchaffin17/AirPollutionFinalProject/blob/master/4.UnsupervisedAnalysis.ipynb)
This notebook contains work done generating clusters of urban areas given their pollutant profiles. Furthermore, it looks at differences in environmental and demographic variables between the clusters.

[**UnsupervisedLearning_pt2.ipynb**](https://github.com/mchaffin17/AirPollutionFinalProject/blob/master/5. UnsupervisedLearning_pt2.ipynb)
This notebook seeks to extend cluster identities to US cities that are missing values for some pollutants using KNN. Additionally, it investigates whether French cities fall within the clusters generated with US cities to generalize these pollutant profiles beyond the US.

##Data Files in this Repository
There are many data files found in the [**Data**](https://github.com/mchaffin17/AirPollutionFinalProject/tree/master/Data) folder of this repository. There are 14 in total:<br>
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
11. dfClusters_kMeans.csv - A file indicating which cluster each US city fell in <br>
12. clustesr_knn.csv - A file indicating cluster identity inferred for many cities through KNN <br>
13. cluster_knn_france.csv - Inferring French city cluster id with US clusters by KNN <br>
14. PollutantFilteringTableau.csv - A file that was used to generate the tableau image that can filter maps based on pollutants <br>
 

##Image Files
This file is found in the Image folder in this repository<br>
1. TransitMap.png - an image file that's used within the EDA notebook

##Project Website and Video Links
The project website can be found at: http://cs109airpollution.github.io<br>
The video can be found at: FILL THIS IN
