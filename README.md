# Project 1
Our group has three visualizations.
## Team Members
Group 3: Viv Lai, Chao-Chun Hsu, & Yichen Wang

## 1. Languages used and the technical terms understanding
![plot](https://i.imgur.com/GIlfGBe.png)
### Overview
This plot is to discover the relationship between languages used and the technical terms understanding. At first, all languages are showing in the plot. Users can then selcet sepcific languages to make a clear comparison. 

### Design Processing
The question we want to ask in this visualization is that does language used affect people recive these knowledge of technical terms? For example, if people learn these ideas in Chinese, it would be difficult for them to relate to these English terms even if they are identical. Thus, considering that comparison matters, the bar char would be a perfect choice. We add the interactive languages selection because it is more clear to compare two languages at once and some times people will only care about the language they are interested in. 

### Observation
After building this representation, we found that people using English and German are more comfortable explaining these terms to their friend. However, when it comes to "
ed device", other language users become comparable and even perform better. By exploring the data with our plot, the original hypothesis on "language would be the barrier for people to recognize these terms" do not hold. The future direction would be discover the educational level or network coverage rate for these users.

### Preprocessing 
I first select the columns containing language and tech terms. Then, I compute the ratio of people feeling comfortable explaining a tech term to a friend for different language. The code is in `preprocessing.ipynb` which can be opened by jupyter notebook. Notes that original csv file is not included in ths dir because of the size limitation. Please add the original csv to this dir before runing the code.

### Sources ##
Grouped bar chart: https://bl.ocks.org/bricedev/0d95074b6d83a77dc3ad
Multiple Select: https://www.jqueryscript.net/form/jQuery-Plugin-For-Easy-Select-Button-Group-ui-choose.html

## 2. Smart devices owned by respective countries
![plot](https://i.imgur.com/AQnVWQL.png)
### Overview
This chart shows the counts of various smart devices owned by respective countries.

When clicked on one of the circles representing one of the smart devices, the chart shows different sizes of bubbles that corresponds to the counts of respective device owned by respective countries.

The user is able to gather bird's eye view insights of the data just by clicking on the different circles. When clicking on any circles, it will show the name of the country, and the exact count of device own.

### Design Processing
In this plot, we want to know how many smart devices do people in one country hold? To investigate this idea, it would be possible to present it with a bar chart which is straightforward to show the difference between different countries. However, it's interesting to see how geography influences these numbers. That's the reason we choose to present geospatial information for different countries. Also, the area the circle represents the quantitative results of our data that is useful for users to compare with different countries.

### Preprocessing
Some of the regions e.g., most of french-owned places are not included in `world_population.tsv`. Preprocessing is done in the following file `preprocess.ipynb`.

### Acknowledgement
The source code is modified from this repo (https://gist.github.com/micahstubbs/8e15870eb432a21f0bc4d3d527b2d14f).

## 3. Factors affecting technology devices buying decisions in different countries 
### Overview
This plot is using a stacked bar chart to show the relationship between the factors influcing their technology devices buying decisions and different countries. When placing mouse over bars, the percentage of that factor will show. The percentage means the ratio of people who consider that factor as the top factor (for that country). Only countries with top 19 survey counts are selected.

### Design Processing
We want to know which factor(s) do people consider important when buying tech devices. At first, we only thought about plot the top 1 factor of each country. However, after examining the dataset we found some factors have similar ratio, so a chart showing all factors' ratios came into our minds. Since we also want to compare accross countries, pie chart will not be used because it's not easy to directly compare the ratios accross different countries, so a visualization which can not only compare ratios within countries but accross is needed. That's where stacked bar chart comes in.

### Observation
Price, features and convenience are top factors and recommendations are not that important. In France and Belgium, convenience is the top one, while price and features are top ones in other countries.

### Preprocessing 
First, delete invalid responses (NaN), then calculate total responses of different countries and select the top 19 countries. Second, group by the countries and count the ratio of people selecting "1" for each factor.
### Reference ##
https://observablehq.com/@d3/stacked-bar-chart

## Your team roles for each individual 
Chao-Chun Hsu: Languages used and the technical terms understanding  
Vivian Lai: Smart devices owned by respective countries  
Yichen Wang: Factors affecting technology devices buying decisions in different countries  
## How to run your code
It's the same as in class acitivity.
In the main folder, run `python -m http.server`.
