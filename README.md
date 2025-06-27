# EDA_analysis

📁 File Name: EDA_Pra.ipynb

🧾 Objective:
 Perform Exploratory Data Analysis (EDA) on a dataset with both numerical and categorical variables. Use visualizations and summary statistics to understand the distribution, relationships, and possible data issues.

🪜 Steps Performed in the Notebook

1. Importing Required Libraries
          📌 These are the core libraries for:
          Data manipulation (pandas)
          Data visualization (seaborn and matplotlib)

2. Loading the Dataset
          📌 Loads the dataset into a DataFrame df from the file data.csv.

3. Initial Data Inspection
          📌 Gives an overview of:
          First 5 rows
          Data types and missing values
          Summary statistics for numeric columns

4. Univariate Analysis
          🔹 Numerical Columns
          sns.histplot(df['Price'], kde=True)
          plt.show()
          📌 Shows distribution of Price.
          🔹 Categorical Columns
          sns.countplot(x='Product', data=df)
          plt.show()
          📌 Shows count of each product type.

5. Bivariate Analysis
          🔹 Categorical vs Numerical
          sns.boxplot(x='Product', y='Price', data=df)
          plt.show()
          📌 Compares price distribution across products.
          🔹 Correlation Matrix
          sns.heatmap(df.corr(), annot=True, cmap='coolwarm')
          plt.show()
          📌 Visualizes correlation between numerical columns.

