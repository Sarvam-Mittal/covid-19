Covid-19 Analysis
==============================

Analysis of Covid-19

Project Organization
------------

    ├── LICENSE
    ├── Makefile           <- Makefile with commands like `make data` or `make train`
    ├── README.md          <- The top-level README for developers using this project.
    ├── data
    │   ├── external       <- Data from third party sources.
    │   ├── interim        <- Intermediate data that has been transformed.
    │   ├── processed      <- The final, canonical data sets for modeling.
    │   └── raw            <- The original, immutable data dump.
    │
    ├── docs               <- A default Sphinx project; see sphinx-doc.org for details
    │
    ├── models             <- Trained and serialized models, model predictions, or model summaries
    │
    ├── notebooks          <- Jupyter notebooks. Naming convention is a number (for ordering),
    │                         the creator's initials, and a short `-` delimited description, e.g.
    │                         `1.0-jqp-initial-data-exploration`.
    │
    ├── references         <- Data dictionaries, manuals, and all other explanatory materials.
    │
    ├── reports            <- Generated analysis as HTML, PDF, LaTeX, etc.
    │   └── figures        <- Generated graphics and figures to be used in reporting
    │
    ├── requirements.txt   <- The requirements file for reproducing the analysis environment, e.g.
    │                         generated with `pip freeze > requirements.txt`
    │
    ├── setup.py           <- makes project pip installable (pip install -e .) so src can be imported
    ├── src                <- Source code for use in this project.
    │   ├── __init__.py    <- Makes src a Python module
    │   │
    │   ├── data           <- Scripts to download or generate data
    │   │   └── make_dataset.py
    │   │
    │   ├── features       <- Scripts to turn raw data into features for modeling
    │   │   └── build_features.py
    │   │
    │   ├── models         <- Scripts to train models and then use trained models to make
    │   │   │                 predictions
    │   │   ├── predict_model.py
    │   │   └── train_model.py
    │   │
    │   └── visualization  <- Scripts to create exploratory and results oriented visualizations
    │       └── visualize.py
    │
    └── tox.ini            <- tox file with settings for running tox; see tox.testrun.org


--------

<p><small>Project based on the <a target="_blank" href="https://drivendata.github.io/cookiecutter-data-science/">cookiecutter data science project template</a>. #cookiecutterdatascience</small></p>

Introduction
------------

On 31 December 2019, WHO was alerted to several cases of pneumonia in Wuhan City, Hubei Province of China. The virus did not match any other known virus. This raised concern because when a virus is new, we do not know how it affects people and this COVID-19 was identified as the cause of an outbreak of respiratory illness first detected in Wuhan, China. Early on, many of the patients in the outbreak in Wuhan, China reportedly had some link to a large seafood and animal market, suggesting animal-to-person spread. However, a growing number of patients reportedly have not had exposure to animal markets, indicating person-to-person spread is occurring.

In India the first COVID-19 case was reported on 30 January in a student who arrived in Kerala state from Wuhan. Then 2 more cases were reported in the next 2 days in Kerala again. For almost a month, no new cases were reported in India, however, on 8th March, five new cases of coronavirus in Kerala were again reported and since then the cases have been rising affecting 14 states. 

Business Understanding
----------------------
Have to use EDA to find out how this COVID has spread in China , Wuhan, Rest of the World and in India along with its neighbouring countries too.More specfically in India 
like how many cases per day, travel history of patients and how much hospital beds are available and till now how much people have been tested positived, recovered or have lost their lives.And Analyzse and understnd the spread od COVID-19 in India , reason , hypotheses which are prevailing mow a days.Basically in depth analysis to touch every aspect of the virus.

Data
----
The data used in the analysis has been gathered from the various sources , brief description of the data in mentioned below and the detail description is mentioned in the data dictionary. All the data mentioned below id updated everyday on hourly basis

- covid_19_clean_complete.csv 

The file contains the cumulative count of confirmed, death and recovered cases of COVID-19 from different countries from 22nd January 2020

- covid_19_data.csv

Johns Hopkins University has made an excellent dashboard using the affected cases data. Data is extracted from the google sheets associated and made available here.The github link of the data is https://github.com/CSSEGISandData/COVID-19.git and the link for the dashboard is https://gisanddata.maps.arcgis.com/apps/opsdashboard/index.html#/bda7594740fd40299423467b48e9ecf6

This dataset has daily level information on the number of affected cases, deaths and recovery from 2019 novel coronavirus. Please note that this is a time series data and so the number of cases on any given day is the cumulative number.

- COVID_open_line_list_data.csv
This file is obtained from https://docs.google.com/spreadsheets/d/1itaohdPiAeniCXNlntNztZ_oRvjh0HsGuJXUJWET008/edit#gid=0 and this is indiviual level data

- COVID19_line_list_data.csv
This files is obtained from https://docs.google.com/spreadsheets/d/e/2PACX-1vQU0SIALScXx8VXDX7yKNKWWPKE1YjFlWc6VTEVSN45CklWWf-uWmprQIyLtoPDA18tX9cFDr-aQ9S6/pubhtml and this is individual level data

- COVID19 India Complete Dataset April 2020.xlsx
Has the complete details of the COVID19 situation in India. Starting from the patient's travel history, to testing count, growth rate, etc. link for the data 
https://www.covid19india.org/

- IndividualDetails.csv
Individual level details are present in IndividualDetails.csv file and is obtained from http://portal.covid19india.org/

- Covid cases in India.csv
Deatils of cases in India State/UT wise.(https://www.worldometers.info/coronavirus/country/india/ and https://www.mohfw.gov.in/)

- per_day_cases.xlsx
daily cases in India(https://www.worldometers.info/coronavirus/country/india/ and https://www.mohfw.gov.in/)

- population_by_country_2020.csv
The data has been scraped from the worldometer


Expectation
-----------
The main exepectation from this analysyis is to get an details overview of COVID-19 in India and in Rest of World by touching each and every scenario and create a report on daily basis and compare the report till a stable figure is reached beacuse as of now we don't know about future aspect of COVID-19.

Further Expantion of the Analysis
---------------------------------
We can try to create a model using Machine Learning Algortihm and use of Healthcare Domain to predict or to get an idea when it will end or how long it will take.

