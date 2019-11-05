This plot is to discover the relationship between languages used and the technical terms understanding. At first, all languages are showing in the plot. Users can then selcet sepcific languages to make a clear comparison. 

The question we want to ask in this visualization is that does language used affect people recive these knowledge of technical terms? For example, if people learn these ideas in Chinese, it would be difficult for them to relate to these English terms even if they are identical. Thus, considering that comparison matters, the bar char would be a perfect choice. We add the interactive languages selection because it is more clear to compare two languages at once and some times people will only care about the language they are interested in. 

Obersivation:
After building this representation, we found that people using English and German are more comfortable explaining these terms to their friend. However, when it comes to "connected device", other language users become comparable and even perform better. By exploring the data with our plot, the original hypothesis on "language would be the barrier for people to recognize these terms" do not hold. The future direction would be discover the educational level or network coverage rate for these users.

Preprocessing:
I first select the columns containing language and tech terms. Then, I compute the ratio of people feeling comfortable explaining a tech term to a friend for different language. The code is in `preprocessing.ipynb` which can be opened by jupyter notebook. Notes that original csv file is not included in ths dir because of the size limitation. Please add the original csv to this dir before runing the code.

Sources:
Grouped bar chart: https://bl.ocks.org/bricedev/0d95074b6d83a77dc3ad
Multiple Select: https://www.jqueryscript.net/form/jQuery-Plugin-For-Easy-Select-Button-Group-ui-choose.html
