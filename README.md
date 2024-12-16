# Data Visualization Final Project - COSI 116A - Group 13
### GitHub Pages Website
https://deborahengelberg.github.io/COSI116A-Brandeis-InfoVis-Fall23.github.io/ 

### Team Members
Debbie Engelberg, Cameron Sherman, Noam Reiner, Mackenzie Chung

### Teaching Staff
Prof. Cashman and TA Aby Iberkleid Szainrok

### Project's Primary Purpose

Our project focuses on visualizing and analyzing how alcohol consumption rates across various countries influence death rates, comparing these impacts to other leading causes of death over multiple years. By highlighting the relationship between alcohol consumption and mortality, this project aims to support healthcare professionals and prevention practitioners in reducing drinking-related risks, offering valuable data to observe and compare global trends.


## SetUp
1. Clone this repository to your local machine. E.g., in your terminal / command prompt `CD` to where you want this the folder for this activity to be. Then run `git clone <YOUR_REPO_URL>`

1. `CD` or open a terminal / command prompt window into the cloned folder.

1. Start a simple python webserver. E.g., one of these commands:
    * `python -m http.server 8000`
    * `python3 -m http.server 8000`
    * `py -m http.server 8000`
    
    If you are using Python 2 you will need to use `python -m SimpleHTTPServer 8000` instead, but please switch to Python 3 as [Python 2 will be sunset on 2020.01.01](https://www.python.org/doc/sunset-python-2/).

1. Wait for the output: `Serving HTTP on 0.0.0.0 port 8000 (http://0.0.0.0:8000/)`

1. Now open your web browser (Firefox or Chrome) and navigate to the URL: http://localhost:8000

## Execution
### Languages and Libraries Used

* JavaScript
* HTML
* CSS
* Python
* JSON
* Pandas
* D3.js



#### <ins> Step 1 - Brainsotrming Ideas  and Looking for Data</ins>

As a group, we quickly decided that we wanted to implement a map visualization in our final project. Our initial idea was to show different types of transportation and their frequencies around the world. However, as we began searching for data, we quickly realized that it was very difficult to find free, accurate transportation data. As a result, we shifted our focus to another type of global data. While researching, we discovered data related to alcohol consumption and causes of death, and we became curious about whether there might be a correlation between the two. This led us to combine these two data sets for our final project.
<br />

#### <ins> Step 2 - Data Cleaning</ins>

For the data cleaning we used Python's Panadas library. We combined four datasets: one on causes of death and three on alcohol consumption. For the cause of death data, we cleaned unnecessary columns, filled null cells, added a total count column, and standardized data types. The alcohol consumption datasets were reformatted and aligned, ensuring consistency for merging. After integrating the datasets by year and country. For interaction with the Json of the map, we added alpha-2 countries codes.

* Link to data cleanning: [Google Colab - Data Cleaning](https://colab.research.google.com/drive/1CXzDcB9EuiBlps0GL37_qgG_ykGpNrow?usp=sharing)
<br />


## Visualization Demonstrations
### Visualization 1: Brushing & Linking
<img src="Images/vis1demo.gif" alt="Visualization 1 Demo" width="600" />

This is our first visualization, which uses three types of charts: a map, a line chart, and a bar chart, all connected through linking and brushing.

* The map displays the distribution of alcohol consumption across the world for a selected year.
* The line chart examines death rates over the years.
* The bar chart shows alcohol consumption trends over the years.
  
When a user selects a year on the map, the corresponding year is highlighted in both the line chart and the bar chart. Similarly, selecting multiple years in the line chart or bar chart highlights them in the other chart through brushing and linking.
Additionally, the map includes a play feature that cycles through the years at set intervals, dynamically updating the highlights in the line and bar charts to reflect the current year.

### Visualization 2: PLACEHOLDER
![Visualtion 1 Demo](Images/vis1demo.gif)


### Visualization 3: Brushing & Linking
<img src="Images/gif-3.gif" alt="Visualization 3 Demo" width="600" />
