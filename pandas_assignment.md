# PandasAssignment

<b> Q1. How do you load a CSV file into a Pandas DataFrame? </b>
```
# Pandas have read_function that can be used to read the csv data
pd.read_csv(file_path)
```

</br>

<b> Q2. How do you check the data type of a column in a Pandas DataFrame? </b>
```
# dtypes can be used to check data type of a column in a Pandas DataFrame
print(pd.DataFrame([[1,2,3],["ds"]]).dtypes)
```

<b> Q3. How do you select rows from a Pandas DataFrame based on a condition? </b>
```
# we can perform conditional operations on the columns and this will return Series which will have binary values, this binary values can be passed to df inside square brackets, such way we can filter rows in pandas

df = pd.DataFrame([[1,2,3],["ds"]])
df[df[0] == 5]

```

<b> Q4. How do you rename columns in a Pandas DataFrame? </b>
```
# we can use rename() method to renmae columns in a Pandas DataFrame

import pandas as pd

# Load a DataFrame
df = pd.read_csv("data.csv")

# Rename a single column
df.rename(columns={'old_name': 'new_name'}, inplace=True)

```
<b> Q5. How do you drop columns in a Pandas DataFrame? </b>
```
# we can use the DataFrame.drop() method.
import pandas as pd

df = pd.read_csv("data.csv")

df.drop(columns=['col_name'], inplace=True)
```

<b> Q6. How do you find the unique values in a column of a Pandas DataFrame? </b>
```
# we can use the unique() method of the Series object.

import pandas as pd

# Load a DataFrame
df = pd.read_csv("data.csv")

unique_values = df['col_name'].unique()
```

<b> Q7. How do you find the number of missing values in each column of a Pandas DataFrame? </b>
```
# we can use the isnull() method and the sum() method.

import pandas as pd

# Load a DataFrame
df = pd.read_csv("data.csv")

# Find the number of missing values in each column
num_missing = df.isnull().sum()

print(num_missing)
```

<b> Q8. How do you fill missing values in a Pandas DataFrame with a specific value? </b>
```
# we can use  can use the fillna() method.
import pandas as pd

# Load a DataFrame
df = pd.read_csv("data.csv")

# Fill missing values with 0
df.fillna(0, inplace=True)
```

Q9. How do you concatenate two Pandas DataFrames?
```
# we can use the concat() method 

import pandas as pd

# Load the first DataFrame
df1 = pd.read_csv("data1.csv")

# Load the second DataFrame
df2 = pd.read_csv("data2.csv")

# Concatenate the two DataFrames
df = pd.concat([df1, df2])

```
<b> Q10. How do you merge two Pandas DataFrames on a specific column? </b>
```
# To merge two Pandas DataFrames on a specific column, we can use the merge() function from the pandas library.

import pandas as pd

# Load the first DataFrame
df1 = pd.read_csv("data1.csv")

# Load the second DataFrame
df2 = pd.read_csv("data2.csv")

# Merge the two DataFrames on the 'col_name' column
df = pd.merge(df1, df2, on='col_name')

```

<b> Q11. How do you group data in a Pandas DataFrame by a specific column and apply an aggregation function? </b>
```
#To group data in a Pandas DataFrame by a specific column and apply an aggregation function, you can use the groupby() method and the agg() method.

import pandas as pd

# Load a DataFrame
df = pd.read_csv("data.csv")

# Group the data by the 'col_name' column and compute the mean of each group
mean_by_group = df.groupby('col_name').mean()

print(mean_by_group)

```

<b> Q12. How do you pivot a Pandas DataFrame? </b>
```
# To pivot a Pandas DataFrame, you can use the pivot_table() function.

import pandas as pd

# Load a DataFrame
df = pd.read_csv("data.csv")

# Pivot the DataFrame
pivoted = df.pivot_table(index='col_name_1', columns='col_name_2', values='col_name_3')

print(pivoted)


```
<b> Q13. How do you change the data type of a column in a Pandas DataFrame? </b>
```
# we can use the astype() method of the Series object.
import pandas as pd

# Load a DataFrame
df = pd.read_csv("data.csv")

# Change the data type of the 'col_name' column to 'float'
df['col_name'] = df['col_name'].astype('float')

```

<b> Q14. How do you sort a Pandas DataFrame by a specific column? </b>
```
# we can use the sort_values() method.

import pandas as pd

# Load a DataFrame
df = pd.read_csv("data.csv")

# Sort the DataFrame by the 'col_name' column
df.sort_values(by='col_name', inplace=True)


```
<b> Q15. How do you create a copy of a Pandas DataFrame? </b>
```
# To create a copy of a Pandas DataFrame, we can use the copy() method.

import pandas as pd

# Load a DataFrame
df = pd.read_csv("data.csv")

# Create a copy of the DataFrame
df_copy = df.copy()
```

Q16. How do you filter rows of a Pandas DataFrame by multiple conditions?
```
#To filter rows of a Pandas DataFrame by multiple conditions, you can use the & operator to specify multiple conditions in the boolean indexing technique.

import pandas as pd

# Load a DataFrame
df = pd.read_csv("data.csv")

# Filter the DataFrame to keep only the rows that meet condition 1 and condition 2
df = df[(df['col_name_1'] > value_1) & (df['col_name_2'] == value_2)]

```
<b> Q17. How do you calculate the mean of a column in a Pandas DataFrame? </b>
```
#To calculate the mean of a column in a Pandas DataFrame, you can use the mean() method of the Series object.

import pandas as pd

# Load a DataFrame
df = pd.read_csv("data.csv")

# Calculate the mean of the 'col_name' column
mean_value = df['col_name'].mean()

print(mean_value)

```

<b> Q18. How do you calculate the standard deviation of a column in a Pandas DataFrame? </b>
```
#To calculate the standard deviation of a column in a Pandas DataFrame, you can use the std() method of the Series object.

import pandas as pd

# Load a DataFrame
df = pd.read_csv("data.csv")

# Calculate the standard deviation of the 'col_name' column
std_value = df['col_name'].std()

print(std_value)

```

<b> Q19. How do you calculate the correlation between two columns in a Pandas DataFrame? </b>
```
# To calculate the correlation between two columns in a Pandas DataFrame, you can use the corr() method of the DataFrame object.

import pandas as pd

# Load a DataFrame
df = pd.read_csv("data.csv")

# Calculate the Pearson correlation between the 'col_name_1' and 'col_name_2' columns
corr = df['col_name_1'].corr(df['col_name_2'])

print(corr)

```

<b> Q20. How do you select specific columns in a DataFrame using their labels? </b>
```
#To select specific columns in a Pandas DataFrame using their labels, you can use the [] operator or the dot notation.

import pandas as pd

# Load a DataFrame
df = pd.read_csv("data.csv")

# Select the 'col_name_1' and 'col_name_2' columns
selected_columns = df[['col_name_1', 'col_name_2']]

print(selected_columns)


```

<b> Q21. How do you select specific rows in a DataFrame using their indexes? </b>
```
# To select specific rows in a Pandas DataFrame using their indexes, you can use the iloc[] or loc[] method.

import pandas as pd

# Load a DataFrame
df = pd.read_csv("data.csv")

# Select rows 0, 1, and 2
selected_rows = df.iloc[0:3]

print(selected_rows)

```

<b> Q22. How do you sort a DataFrame by a specific column? </b>
```
# we can use the sort_values() method.

import pandas as pd

# Load a DataFrame
df = pd.read_csv("data.csv")

# Sort the DataFrame by the 'col_name' column
df.sort_values(by='col_name', inplace=True)


```

<b> Q23. How do you create a new column in a DataFrame based on the values of another column? </b>
```
# To create a new column in a Pandas DataFrame based on the values of another column, you can use the apply() method and a lambda function.

import pandas as pd

# Load a DataFrame
df = pd.read_csv("data.csv")

# Create a new column 'new_col' based on the values of the 'col_name' column
df['new_col'] = df['col_name'].apply(lambda x: x * 2)

```

<b> Q24. How do you remove duplicates from a DataFrame? </B>
```
# To remove duplicates from a Pandas DataFrame, you can use the drop_duplicates() method.

To remove duplicates from a Pandas DataFrame, you can use the drop_duplicates() method.

import pandas as pd

# Load a DataFrame
df = pd.read_csv("data.csv")

# Remove duplicates
df = df.drop_duplicates()

```

</b> Q25. What is the difference between .loc and .iloc in Pandas?</b>
```
# In Pandas, .loc is used to access rows and columns by labels, while .iloc is used to access rows and columns by integer indices.

import pandas as pd

df = pd.DataFrame({'A': [1, 2, 3], 'B': [4, 5, 6], 'C': [7, 8, 9]},
                  index=['a', 'b', 'c'])

value = df.loc['a', 'A']
value = df.iloc[0, 0]                

```