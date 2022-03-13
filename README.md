# Learn Machine Learning
## ML Tools
### 1. Pandas
Data manipulation & analysis package.
* cheat sheet: https://github.com/GokuMohandas/MadeWithML/blob/4ad626098aca25db5628fe67895e738d5a5c2c2a/notebooks/03_Pandas.ipynb
### 2. Matplot
Data Visualization
### 3. Seaborn
Data Visualization. [Ref](https://seaborn.pydata.org/)
```
import seaborn as sns
sns.set()

graph = sns.scatterplot(x='Wage', y='Value', data=df1)
graph
```
### 4. Bokeh
Interactive Data Visualization. [Ref](https://docs.bokeh.org/en/latest/index.html)
```
from bokeh.plotting import figure,show,output_notebook
from bokeh.models import HoverTool

# output to notebook
output_notebook()

TOOLTIPS = HoverTool(tooltips=[
    ("index", "$index"),
    ("(Wage,Value)", "(@Wage, @Value)"),
    ("Name", "@Name")]
)

p = figure(title="Soccer 2019", x_axis_label='Wage', y_axis_label='Value', plot_width=700, plot_height=700, tools=[TOOLTIPS])
p.circle('Wage', 'Value', size=10, source=df1)
show(p)
```
### 5. Scikit Learn
Machine learning library. [Ref](https://scikit-learn.org/stable/)

#### Model Persistence
To save a model after training: [Ref](https://scikit-learn.org/stable/modules/model_persistence.html)  
Sample notebook [here](https://github.com/aneagoie/ML-Notes/blob/master/iris.ipynb)

### 6. ImageAI
Tensorflow based Open Source Python Library for DL & Computer Vision. [Ref](https://github.com/OlafenwaMoses/ImageAI)

## References
* [ML Data Science notebook](https://github.com/aneagoie/ML-Notes/blob/master/soccer.ipynb)
* [Nearest Neighbour](https://scikit-learn.org/stable/modules/neighbors.html#nearest-neighbors-classification)