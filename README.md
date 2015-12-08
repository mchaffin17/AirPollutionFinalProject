# AirPollutionFinalProject
##Background and Motivation
The World Health Organization reported that in 2012 about 7 million people died as a result of air pollution exposure, a finding that was more than double previous estimates.  According to the WHO, this finding “confirms that air pollution is now the world’s largest single environmental health risk.”  Air pollution can lead to a variety of potentially fatal conditions such as heart disease, stroke, COPD, and lung cancer.  Thus it is critical that more research on air pollution causes and interventions to reduce such pollution be done.
 
As students at the Harvard T.H. Chan School of Public Health, we want to conduct some research into air pollution in the USA as well as on some of the determinants of such pollution such as weather, commuting, and population density given the severity of this public health issue.  By understanding the pollutant profiles of various cities, more targeted and effective interventions for reducing pollution on a by-pollutant-type basis could then be proposed and implemented.  Linking these specific profiles to certain determinants would also aid in the creation of powerful air pollution reduction policies.  These various analyses could be useful for developing legislation across the USA.  Additionally, we could predict the pollutant profiles of cities in the third world, where such measuring of pollutants is not available, based on weather, population, etc.  Such prediction would allow for better formulation of air pollution reduction policies for those cities.
Initial Questions:<br>
<ol>
<li>Are there certain pollutant profiles that characterize groups of US cities?</li>
<li>What is the distribution of pollutants (air particulate matter, gas levels, etc.) within these clusters?</li>
<li>What are the determinants (weather, demographics, transportation, etc.) of these pollutant profiles?</li>
<li>Can we use data on weather, demographics, transportation, etc. to predict a city’s pollutant profiles?</li>
<li>Can specific policy recommendations be made based on a city’s pollutant profile?</li>
</ol>

##Related Work
We were partly inspired by this interesting visualization that shows the relative contribution different environmental and anthropogenic factors on climate change trends.<br>
http://www.bloomberg.com/graphics/2015-whats-warming-the-world/?utm_source=The+Weekly+Pique&utm_campaign=cf7d4cd5ac-Episode+12%3A+Global+Warming&utm_medium=email&utm_term=0_4627876a86-cf7d4cd5ac-297062977

##Key Findings
Based on our analysis, air quality appears to be a composite of many features, some related to human activity and some related to environmental sources. The relative contribution of these two sources seems to vary across pollutants which has implications about how to design effective overall air quality interventions. Using multiple modeling approaches, we find that some pollutant concentrations, such as NO2 and O3, are easier to predict than others.<br>
·       Airborne NO2, PM2.5, and O3 of cities can be somewhat predicted based on demographic and weather features, but PM10, CO, and SO2 are not well described from these characteristics<br>
·       Prediction models based on US cities do not extend well to French cities<br>
·       The relative importance of anthropogenic and environmental factors to air pollutant concentrations varies between pollutants<br>
·       Distinct types of cities exist that can be characterized by their particular pollutant profiles<br>
        ·       These clusters can be differentiated by liquid precipitation, air pressure, temperature, and land area<br>
·       Differential patterns of missing pollutant data for US cities made imputation of clusters unreliable.<br>
·       When French cities were clustered with the same method, their pollutant profiles looked reasonably similar to the clustered US pollutant profiles.

##Notebooks in this repository
There are several ipython notebooks in this repository. These are designed to break up the individual sections of the project into smaller, self-contained processes. To follow the project process, the optimal order to view these files is:<br>
1. DataCollection&Cleaning.ipynb<br>
2. ExplotatoryDataAnalysis.ipynb<br>
3. PredictiveLinearModeling.ipynb<br>
4. UnsupervisedAnalysisPart1.ipynb<br>
5. UnsupervisedAnalysisPart2.ipynb<br>

Each section contains the following information.

[**DataCollection&Cleaning.ipynb**](https://github.com/mchaffin17/AirPollutionFinalProject/blob/master/DataCollection%26Cleaning.ipynb)
This notebook contains the details of data collection and scraping. All files used in this process are either accessed directly from their links within the notebook or contain in the dropbox repository found at: https://www.dropbox.com/sh/cd95rdgrbm9cpz7/AAAG9758zR1tUMvGsxKtIJzXa?dl=0.

[**ExploratoryDataAnalysis.ipynb**](https://github.com/mchaffin17/AirPollutionFinalProject/blob/master/ExploratoryDataAnalysis.ipynb)
This notebook contains the basic visualizations of the data and simple bivariate analyses.

[**PredictiveLinearModeling.ipynb**](https://github.com/mchaffin17/AirPollutionFinalProject/blob/master/PredictiveLinearModeling.ipynb)
This notebook works to build predictive models of the individual pollutants based on demographic and environmental variables. Analysis was validated using cities in France.

[**UnsupervisedAnalysis.ipynb**](https://github.com/mchaffin17/AirPollutionFinalProject/blob/master/UnsupervisedAnalysis.ipynb)
This notebook works to generate particular clusters of urban areas given their pollutant profiles. Furthermore, it looks at differences in environmental and demographic variables between the clusters.

[**UnsupervisedAnalysis_pt2.ipynb**](https://github.com/mchaffin17/AirPollutionFinalProject/blob/master/UnsupervisedLearning_pt2.ipynb)
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
12. PollutantFilteringTableau.csv - A file that was used to generate the tableau image that can filter maps based on pollutants <br>

##Other files
Beyond these files, there are several image files used throughout notebooks

##Project Website and Video Links
The project website can be found at: http://cs109airpollution.github.io<br>
The video can be found at: FILL THIS IN
