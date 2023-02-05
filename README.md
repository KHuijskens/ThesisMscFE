# ThesisMscFE: BelastingTelefoon
This repository contains the source code for my Master's thesis in Tax Economics. 
The goal of my thesis is to explore the relationship between tax complexity and the number of calls received by the tax authorities (BelastingTelefoon). 
The data contains information regarding the calls received from 2nd of January 2019 onwards. Due to the starting date of my thesis, the date range that is used 
is 02-01-2019 until 30-08-2022. The data can be found at https://www.belastingdienst.nl/wps/wcm/connect/bldcontentnl/themaoverstijgend/brochures_en_publicaties/open_data_beltel_wachtrij.

The first file, THESIS-FINAL-CONCEPT-ANALYSIS, contains the data transformation and EDA steps. 
First, the data is cleaned (removal of outliers, removal of a discontinued theme). 
Then, the themes are analysed by looking at the moving averages of calls over time, waiting times and by comparing each theme's complexity scores
with their rank based on amount of calls. 

In the second file, THESIS-FINAL-CONCEPT-MODEL, the data is enriched with the dates of tax deadlines, Prinsjesdag, national holidays and the weather. 
The enriched dataset is explored by visualising the tax deadlines against the amounts of calls, to see if any effect is visible. 
Finally, a model is presented for each theme using GridSearchCV. These models are assumed to reflect the baseline for calls to be expected.
The assumption is made that themes that are more easily predictable are less complex in nature. 
This assumption is used to compare against the literature-based complexity scores.
