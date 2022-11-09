## Covid-19 Dashboard- Python + Tableau

Here, I've tried to create an interactive Covid-19 dashboard using Python and Tableau.

The raw covid data was collected from COVID-19 Data Repository by the Center for Systems Science and Engineering (CSSE) at Johns Hopkins University. Github link to the data repository- https://github.com/CSSEGISandData/COVID-19
At the time of making this dashboard, the dataset has data up to November 07, 2022.

 - **Python Version-** 3.9
 - **Python Packages-** Pandas, Numpy
 - **Application-** Jupyter Notebook & Tableau


The CSSE Covid-19 dataset consists of three tables about daily confirmed, deaths and recoveries cases per country/region. Each table presents the data in wide (crosstab) format, with each day in a column. The dataset is cleansed and preproccessed using python inside a jupyter notebook (Covid_19_Preprocessing_Data.ipynb). The dataset is transformed from wide to long format using the Pandas melt function (for usage suitability inside Tableau).


The refined dataset is later combined with population data (dataset collected from- https://www.kaggle.com/datasets/tanuprabhu/population-by-country-2020) to create the confirmed / population data. In the end, the refined and processed data is saved as a new dataset as *covid19.csv* file.


This *covid19.csv* file is used as the source for my Tableau dashboard. The interactive Tableau dashboard file is provided in the repository as *covid19.twbx*. Also a screenshot of the dashboard is provided here (*Dashboard.png*). ![Covid19 Dashboard](https://github.com/tariquldipu/Covid19-Dashboard/blob/main/Dashboard.png)

The dashboard provides data up to November 07, 2022. The dashboard features an interactive world map with corresponding infos for confirmed, deaths, ongoing, recoveries cases. Clicking on a specific country from the world map, will show the Total Confirmed, Infection Rate, Recovery Rate, Total Deaths, Fatality Rate etc. information on the dashboard.


#python #tableau #numpy #pandas # image #color_detection #python_project #dashboard
