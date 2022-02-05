# SLC_Water_Systems_Analysis
Within this repository are the simulation results and respective Jupyter Notebook analysis tools for the following research abstract:

Enhancing Municipal Water System Planning and Operations Through Climate-Sensitive Demand Estimates

High seasonality and interannual climate patterns drive the western U.S.'s water supply and demand variability. 
While the mean and variance of supply and demand drivers are changing with climate and urbanization, the metrics of reliability, resilience, and vulnerability (RRV) that guide urban water systems (UWS) seasonal management and operations tend to be built on assumptions of stationarity.
In this research, we use documented performance of a real-world UWS as a testbed to investigate how RRV metrics -- and therefore UWS planning and operations guidance --  change in response to demands modeled with and without assumptions of stationarity during dry, average, and wet hydroclimate conditions.
The results indicate an assumption of stationary demands leads to large differences between simulated and observed RRV metrics for all supply scenarios, and especially in supply-limiting conditions when the peak severity is 129\% from the observed.
The management implications of relying on stationary demands are severe: if seasonal operational decisions were made on these model results, managers might over-estimate seasonal out-of-district water requests by 50\%.
In contrast, when using non-stationary demands, one can expect system performance error reduction between 30\% to 60\% for average and dry climate conditions, respectively, and accurate RRV metrics.
Our results further indicate that this UWS is more sensitive to percent changes in per-capita demand relative to percent changes in supply, but because the supply variability is so much greater (158% vs. demand range of 28%), we suggest further work to examine the combined (and coupled) influence of both factors in overall system performance.


The ModelOutput folder contains all monthly scale water demands.
The WD_Scenario_Builder_Monthly2.ipynb loads these demand projections from the CSD-WDM and interpolates them to a daily temporal resolution.
The DroughtSuplusAverage_Data folder contains all SLC-WDM simulation results.
Using the SLC_WSM_Performance_Analyzer_SLv2.ipnyb script, we can load all Goldsim SLC-WSM simulations to determine urban water system Reliability, Resilience, and Vulnerability compared to the historical record.
This scrip also supports figure development and additional analysis functions. 
