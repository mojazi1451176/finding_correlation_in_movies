Movie Dataset Analysis Project
This project is a data analysis exercise that explores a dataset of movies, focusing on data cleaning, transformation, correlation analysis, and visualizations using Python and various data science libraries.

📂 File
python_project2.py: The Python script version of a Jupyter Notebook analyzing a movie dataset (originally from a Google Colab notebook).

📊 Project Objective
To uncover insights from a movie dataset, specifically:

Clean and preprocess the data

Investigate relationships between numeric features like budget, gross earnings, votes, and more

Identify which features most correlate with a movie's success

📚 Libraries Used
pandas: For data manipulation

numpy: For numerical computations

seaborn & matplotlib: For data visualization

🛠️ Steps Performed
Data Import & Initial View

Loads the dataset from a .csv file

Displays initial rows and checks for null values and data types

Data Cleaning

Handles missing values using dropna()

Converts relevant columns (budget, gross, votes, runtime) to integers

Corrects release years extracted from the released column

Strips whitespace from column names and entries

Duplicate Removal

Removes duplicate movie names

Exploratory Data Analysis (EDA)

Creates scatter plots and regression plots to show trends

Computes correlation matrices for numerical features

Visualizes correlations using heatmaps

Categorical Encoding

Converts object (string) type columns to numerical using category codes

Advanced Correlation Analysis

Uses correlation coefficients to unstack and sort relationships

Filters for high correlation values (e.g., budget vs. gross, votes vs. gross)

🔍 Key Findings
Budget and Gross Earnings are strongly positively correlated.

Votes also show high correlation with Gross Earnings, suggesting more popular films tend to earn more.

Encoding categorical features helps uncover additional relationships hidden in the original string data.

📝 Notes
Make sure to update the dataset path (df = pd.read_csv(...)) if you're running this locally.

The script assumes the dataset includes columns such as: budget, gross, votes, runtime, released, name, etc.

