# Reading notes

## Pandas

Explain the purpose and basic functionality of the Pandas library. What are some common operations that can be performed on data using Pandas, and how do they contribute to data analysis and manipulation?

Pandas provides data structures and functions that make it easy to work with structured data, such as spreadsheets, SQL tables, and CSV files. The primary purpose of Pandas is to help users efficiently manage and manipulate data for various data analysis tasks.



User
Explain the purpose and basic functionality of the Pandas library. What are some common operations that can be performed on data using Pandas, and how do they contribute to data analysis and manipulation?
ChatGPT
Pandas is a popular open-source Python library designed for data manipulation and analysis. It provides data structures and functions that make it easy to work with structured data, such as spreadsheets, SQL tables, and CSV files. The primary purpose of Pandas is to help users efficiently manage and manipulate data for various data analysis tasks.

Here are some key aspects of Pandas and common operations performed using the library:

1. Data Structures:

* DataFrame: The core data structure in Pandas is the DataFrame. It is a 2-dimensional, labeled data structure similar to a spreadsheet or SQL table. DataFrames can store data of different types in columns, and they provide powerful indexing and selection capabilities.

* Series: A Series is a one-dimensional array-like object that can store data of any type. Series are often used to represent a single column or row in a DataFrame.

2. Data Import and Export:

* Pandas allows you to read data from various file formats, such as CSV, Excel, SQL databases, JSON, and more. You can also write data back to these formats after manipulation.

* Common functions for importing data include pd.read_csv(), pd.read_excel(), pd.read_sql(), and for exporting, to_csv(), to_excel(), etc.

What are the primary data structures in Pandas, and how do they differ in terms of use cases?

DataFrame:

A DataFrame is a 2-dimensional, tabular data structure that resembles a spreadsheet or a SQL table. It is the most commonly used data structure in Pandas.

Use Cases:

* Storing and manipulating structured data with rows and columns, like a dataset in a CSV file or a database table.
* Performing data operations that involve multiple columns, such as filtering, aggregation, grouping, and merging datasets.
* Visualizing data and creating summary statistics.

```python
import pandas as pd

data = {'Name': ['Alice', 'Bob', 'Charlie'],
        'Age': [25, 30, 22]}
df = pd.DataFrame(data)
```
Series:

A Series is a 1-dimensional data structure that is similar to a column in a DataFrame or an array. It consists of a sequence of values and an associated index.

Use Cases:

* Representing a single column or row of data from a DataFrame.

* Performing operations on individual data series, such as mathematical calculations or applying functions.

* Selecting specific data elements by label or position.


```python
import pandas as pd
ages = pd.Series([25, 30, 22])

```

Describe the process of loading a dataset into a Pandas DataFrame. What are some common file formats that can be used, and which Pandas functions are utilized to read these formats?

Before you can work with Pandas, you need to import it into your Python script or Jupyter Notebook using the import statement:

```python
import pandas as pd

```
Common file formats supported by Pandas include:

CSV (Comma-Separated Values)

To load

```pyton
df = pd.read_csv('your_dataset.csv')

```

Excel (XLSX)

To load

```pyton
df = pd.read_excel('your_dataset.xlsx', sheet_name='sheet_name')

```

SQL (Structured Query Language) databases

To load

```pyton
import sqlite3
conn = sqlite3.connect('your_database.db')
query = 'SELECT * FROM your_table'
df = pd.read_sql(query, conn)

```

JSON (JavaScript Object Notation)

To load

```pyton
df = pd.read_json('your_dataset.json')

```

HDF5 (Hierarchical Data Format)

To load

```pyton
df = pd.read_hdf('your_dataset.h5', key='data')

```

Parquet
```python
df = pd.read_parquet('your_dataset.parquet')

```

HTML (for web scraping)
```python
tables = pd.read_html('url_or_html_file')
df = tables[0]  # Select the appropriate table from the list

```

### Resources

[Pandas in 10](https://pandas.pydata.org/pandas-docs/stable/user_guide/10min.html)

[Chatgpt](https://chat.openai.com/)