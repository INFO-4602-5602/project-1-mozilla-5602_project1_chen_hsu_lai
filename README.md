# Projoect 1
Our group has tree plots.
## Team Members
Group 3: Viv Lai, Chao-Chun Hsu, & Yichen Wang

## 1. Languages used and the technical terms understanding
![plot](https://i.imgur.com/IcpBaCQ.png)
### Overview
This plot is to discover the relationship between languages used and the technical terms understanding. At first, all languages are showing in the plot. Users can then selcet sepcific languages to make a clear comparison. 

### Design Processing
The question we want to ask in this visualization is that does language used affect people recive these knowledge of technical terms? For example, if people learn these ideas in Chinese, it would be difficult for them to relate to these English terms even if they are identical. Thus, considering that comparison matters, the bar char would be a perfect choice. We add the interactive languages selection because it is more clear to compare two languages at once and some times people will only care about the language they are interested in. 

### Obersivation
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

## Your team roles for each individual 

## How to run your code
It's the same as in class acitivity.
`python -m http.server`
