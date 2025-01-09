# Uber-Analysis-Using-Python


_Technologies Used_
_Programming Language:_ Python
_Libraries:_ Pandas, NumPy, Matplotlib, Seaborn

pandas and numpy:
Used for data manipulation and numerical computations.

matplotlib and seaborn: 
Essential for data visualization. This will allow us to create various charts and graphs to explore the dataset visually. 

Load the dataset:

Reads the Uber dataset into a Pandas DataFrame for analysis.
pd.read_csv() allows us to easily load structured data stored in a CSV file.

.head()

Displays the first five rows of the dataset to give you an overview of its structure, column names, and data types.
Helps in understanding what kind of data we're working with before diving deeper.

.shape()

Provides the dimensions of the dataset in terms of rows and columns.
Useful for understanding dataset size and for validating data after cleaning steps.

.info()

Displays metadata about the dataset, such as column names, data types, and the number of non-null (filled) values for each column.
Helps identify missing data and ensure data types are correct for further analysis.

dataset['PURPOSE'].fillna("NOT", inplace=True)

The PURPOSE column had many missing values (only 653 out of 1156 were non-null).
Filling missing values with "NOT" ensures there are no gaps in the dataset, which prevents errors during analysis.
inplace=True updates the original DataFrame directly without creating a new copy.
