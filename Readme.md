
# About the project

The goal of this project is to analyse inspection score data from data.gov/austin and https://data.cityofnewyork.us to see what type of scoring system these cities have and how restaurants and other food places rate according to that. I chose Austin because it was the first dataset I found on restaurant inspection scores. I chose new york because I was curious to find out the scores that were given to the plethora of restaurants present in the big apple.

This README file and the Jupyter Notebook file, Final_project.ipynb, contain the information and
references needed to reproduce the analysis, including a description of the data and all relevant resources
and documentation, with hyperlinks to those resources.

# About the data

The data has been collected from https://data.cityofnewyork.us/Health/DOHMH-New-York-City-Restaurant-Inspection-Results/xx67-kt59 for New York and https://data.austintexas.gov/Health-and-Community-Services/Restaurant-Inspection-Scores/ecmv-9xxi for Austin, Texas.

The Inspection data for Austin has the following columns:  
1) Restaurant Name  
2) Zip code  
3) Inspection Date  
4) Score  
5) Address  
6) Facility ID  
7) Process Description

The Inspection data for New York has 18 columns. Some of them are:  
1) DBA - Restaurant Name
2) BORO - Neighborhood
3) Zip code  
4) Phone  
5) Cuisine  
6) Score  
7) Record Date

The inspection data for Maryland has 16 columns. Some are:
1) business_id
2) business_name
3) inspection_id
4) inspection_result
5) inspection_date

### License

All the data has been taken from data.gov, the official site for open data from the U.S. Government

U.S. Federal data available through Data.gov is offered free and without restriction. Data and content created by government employees within the scope of their employment are not subject to domestic copyright protection under 17 U.S.C. § 105.


# Tools  used in the Project

In addition to the APIs described above, the Jupyter Notebook file in this repository, Final_project.ipynb,
contains the python code to get, parse, save, consolidate, and visualize the data.

Jupyter Notebook can be used under the License BSD 3-Clause License. It is an open-source web application that allows you to create and share documents that contain live code, equations, visualizations and narrative text.

You will need Python 3.X and the following Python libraries to run the code in Final_project.ipynb.

Matplotlib : will be used for data visualization
Pandas : will be used for data processing
Seaborn -- Note: this library was used to make the heatmap and nothing else

If necessary, you can pip install any of the above libraries, for example:
pip install matplotlib or pip3 install matplotlib.

Additionally, if you have any version of Python 3.X installed, you should already have the csv, json,
and requests libraries installed. These dependency libraries will be used to get and save data in the notebook
file, hcds-a1-data-curation.ipynb.

 
