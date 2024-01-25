# Reading Notes

What are the key differences between Matplotlib, Seaborn, and Bokeh libraries in terms of their features and use cases? Provide an example of a specific visualization that is more suitable for each library.

Matplotlib is a versatile library for creating static plots with fine-grained control, Seaborn simplifies statistical visualizations, and Bokeh specializes in interactive web-based visualizations. Your choice of library depends on the specific visualization requirements and the level of interactivity needed for your project.

Examples 

```python
import matplotlib.pyplot as plt

# Sample data
x = [1, 2, 3, 4, 5]
y = [10, 15, 7, 12, 9]

# Create a line plot
plt.plot(x, y)
plt.xlabel('Time')
plt.ylabel('Stock Price')
plt.title('Stock Price Trend')
plt.show()

```

```python
import seaborn as sns
import matplotlib.pyplot as plt

# Sample data
data = sns.load_dataset('tips')

# Create a box plot
sns.boxplot(x='day', y='total_bill', data=data)
plt.xlabel('Day of the Week')
plt.ylabel('Total Bill')
plt.title('Distribution of Total Bills by Day')
plt.show()

```

```python
from bokeh.plotting import figure, show
from bokeh.models import ColumnDataSource, HoverTool

# Sample data
source = ColumnDataSource(data={'x': [1, 2, 3, 4, 5], 'y': [10, 15, 7, 12, 9]})

# Create a scatter plot with interactivity
p = figure(title='Interactive Scatter Plot', tools='hover,pan,wheel_zoom,box_zoom,reset')
p.scatter(x='x', y='y', source=source, size=10, color='blue')

# Add a hover tool for additional information
hover = HoverTool()
hover.tooltips = [('Value', '@y')]
p.add_tools(hover)

show(p)

```


In the Seaborn library, what are the main functions to create relational, categorical, and distribution plots? Briefly explain the purpose of each type of plot and provide an example use case.

**Relational Plots:**

**Function:** sns.relplot()

**Purpose:** Relational plots are used to visualize the relationship between two numeric variables. They are often used for exploring how two variables are correlated or distributed.

**Example Use Case:** Scatter plots, line plots, or any plot that displays the relationship between two numeric variables. For instance, visualizing the relationship between a student's study time and their exam scores.

```python
import seaborn as sns
import matplotlib.pyplot as plt

# Sample data
data = sns.load_dataset('tips')

# Create a scatter plot
sns.relplot(x='total_bill', y='tip', data=data)
plt.xlabel('Total Bill')
plt.ylabel('Tip')
plt.title('Scatter Plot of Total Bill vs. Tip')
plt.show()

```

**Categorical Plots**:

**Functions**: Various functions like sns.catplot(), sns.boxplot(), sns.barplot(), sns.countplot(), etc.

**Purpose**: Categorical plots are used to visualize the distribution of data across categories or to compare different categories. They are particularly useful for exploring patterns in categorical data.

**Example Use Case**: Creating bar charts, box plots, violin plots, or count plots to compare different categories. For example, visualizing the distribution of car types in a dataset.

```python
import seaborn as sns
import matplotlib.pyplot as plt

# Sample data
data = sns.load_dataset('diamonds')

# Create a box plot
sns.boxplot(x='cut', y='price', data=data)
plt.xlabel('Cut')
plt.ylabel('Price')
plt.title('Box Plot of Price by Diamond Cut')
plt.xticks(rotation=45)
plt.show()

```

**Distribution Plots**:

**Functions**: Functions like sns.histplot(), sns.kdeplot(), sns.distplot(), etc.

**Purpose**: Distribution plots are used to visualize the distribution of a single variable. They provide insights into the data's central tendency, spread, and shape.

**Example Use Case**: Creating histograms, kernel density plots, or distribution plots to explore the distribution of a numeric variable. For instance, visualizing the distribution of ages in a population.

```python
import seaborn as sns
import matplotlib.pyplot as plt

# Sample data
data = sns.load_dataset('titanic')

# Create a histogram
sns.histplot(data['age'], bins=20, kde=True)
plt.xlabel('Age')
plt.ylabel('Frequency')
plt.title('Distribution of Passenger Ages on the Titanic')
plt.show()

```

Discuss the role of the Seaborn Cheat Sheet in a Python developer’s workflow. What are some key sections or elements featured in the cheat sheet that can help a developer quickly reference Seaborn functionalities?

he Seaborn Cheat Sheet is a valuable resource for Python developers, particularly those working on data visualization tasks with the Seaborn library. It plays a significant role in a Python developer's workflow by providing quick reference and guidance on Seaborn's functionalities. Here are some key sections and elements featured in the cheat sheet that can help developers:

* *Basic Steps*: The cheat sheet outlines the fundamental steps for creating plots with Seaborn, starting from preparing data to customizing plots. It serves as a concise reminder of the overall workflow.

* *Importing Libraries*: It provides aliases for importing essential libraries like pandas, numpy, matplotlib.pyplot, and seaborn, making it easier to set up the development environment.

* *Plotting With Seaborn*: The cheat sheet includes examples of code snippets for common plotting tasks, such as creating scatter plots, linear regression plots, and setting plot labels and titles. Developers can quickly reference these examples for their own projects.

## Resources

[Matplotlib Tutorial](https://www.labri.fr/perso/nrougier/teaching/matplotlib/)

[Seaborn Tutorial](https://seaborn.pydata.org/tutorial.html)

[Bokeh Tutorial](https://mybinder.org/v2/gh/bokeh/bokeh-notebooks/master?filepath=tutorial%2F00%20-%20Introduction%20and%20Setup.ipynb)

[Seaborn Cheat Sheet](https://s3.amazonaws.com/assets.datacamp.com/blog_assets/Python_Seaborn_Cheat_Sheet.pdf)

[ChatGPT](https://chat.openai.com/)