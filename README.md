<h1>Covid Spread</h1>
<h2>Bonaventure Raj</h2>

<h3>Objective</h3>
<br/>
This repository explores the rate of spread of Covid-19 in Clark County, Nevada. It subsets on data found from Feb 1st, 2020 - Oct 1st, 2021. To better understand the impacts of external factors such as State Policies, and Public Mask Mandate regulations we add these feature by date announced to the visualization. The extension looks at two further questions. 1) How much of an impact did covid have on employment rate, and was it significant at a 0.05 level? 2) How much did this impact the employment rate of the state as a whole?

<br/>
<h3>Structure</h3>
<br/>
This repository has a `data` directory for all acquired and produced data. Further explanation on acquired data is found in the Data section below. The acquired data is produced by `Data_Formatting.ipynb`. `Data_Formatting.ipynb` is a notebook that clean, filters, and aggregates all acquired data needed for the visualization step in `Visualization.ipynb`. That leaves that `Visualization.ipynb` visualizes the time series data that outputs `mask_covid_spread.png` graphic that leads to our conclusion.

The extension of this project covered in `extension_analyze_data.ipynb` and `extension_write_data.ipynb` cover the final two objectives stated above. These objectives contain the analysis and explanation of the code in those notebooks.

<br/>
<h3>Data</h3>
<br/>
**Note** Due to size limits of GitHub repositories, they will not be attached here!
<br/>
All aquired data were found in different sources, hence placed in different directories.
<br/><br/>

`data/case` directory:
<br/>
This acquires data from: https://www.kaggle.com/datasets/antgoldbloom/covid19-data-from-john-hopkins-university, licensed as Attribution 4.0 International (CC BY 4.0). It has several fields in the dataset we use `RAW_us_confirmed_cases.csv` which has timeseries data for all counties for # of covid cases.
<br/><br/>

`data/mandate` directory:
<br/>
This acquires data from: https://data.cdc.gov/Policy-Surveillance/U-S-State-and-Territorial-Public-Mask-Mandates-Fro/62d6-pm5i, licensed as  Apache-2.0 license, and also states that it is public use data. It has several fields on mandates issued per county by date.
<br/><br/>

`data/compliance` directory:
<br/>
This acquires data from: https://github.com/nytimes/covid-19-data/tree/master/mask-use, licensed to The New York Times (for free use, as long as 1) non-commercial and 2) credits the New York Times). We do not use this analysis for commerical reasons and we credit this data used from the New York Times. This is survey data that checks mask-use based on feedback from users on whether they wear a mask as NEVER, RARELY, SOMETIMES, FREQUENTLY, ALWAYS as a proportion per population in county over number of responses.


<h3>References</h3>
https://www.bls.gov/web/metro/laucntycur14.txt
https://www.bls.gov/lau/laucnty20.txt
https://www.nevada-demographics.com/counties_by_population
https://ycharts.com/indicators/las_vegas_nv_unemployment_rate#:~:text=Las%20Vegas%2C%20NV%20Unemployment%20Rate%20is%20at%205.40%25%2C%20compared,long%20term%20average%20of%206.83%25.
https://datausa.io/profile/geo/boulder-city-nv#covid \

https://data.bls.gov/cgi-bin/surveymost