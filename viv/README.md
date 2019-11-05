### Overview
This chart shows the counts of various smart devices owned by respective countries.

When clicked on one of the circles representing one of the smart devices, the chart shows different sizes of bubbles that corresponds to the counts of respective device owned by respective countries.

The user is able to gather bird's eye view insights of the data just by clicking on the different circles. When clicking on any circles, it will show the name of the country, and the exact count of device own.

### Design Processing
In this plot, we want to know how many connected devices do people in one country hold? To investigate this idea, it would be possible to present it with a bar chart which is straightforward to show the difference between different countries. However, it's interesting to see how geography influences these numbers. That's the reason we choose to present geospatial information for different countries. Also, the area the circle represents the quantitative results of our data that is useful for users to compare with different countries.

### Preprocessing
Some of the regions e.g., most of french-owned places are not included in `world_population.tsv`. Preprocessing is done in the following file `preprocess.ipynb`.

### Acknowledgement
The source code is modified from this repo (https://gist.github.com/micahstubbs/8e15870eb432a21f0bc4d3d527b2d14f).


