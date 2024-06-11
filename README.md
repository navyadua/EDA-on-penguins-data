## Exploratory Data Analysis and Clustering Patterns of Penguin Data🐧📊

This repository contains code and documentation for conducting exploratory data analysis (EDA) on a dataset containing information about penguins. The dataset includes variables such as species, island of habitat, bill measurements, body mass, gender, and year of observation.

### Introduction ℹ️
Exploratory Data Analysis (EDA) is a crucial step in understanding the underlying patterns and characteristics of a dataset. In this project, we conduct EDA on a penguin dataset to gain insights into the distribution of penguin species, explore relationships between variables, and identify any interesting patterns or trends.

### Data Preparation 🛠️
We start by loading the necessary libraries and the penguin dataset into a pandas DataFrame. We handle missing values and convert the DataFrame into a SQLite database for easier querying and analysis.

### Basic EDA 📊
Basic EDA is performed using SQL queries to explore the dataset. We count the unique occurrences of species, islands, gender, and years, providing insights into the distribution of these categorical variables. Additionally, we visualize the counts of records by island and species and the gender distribution using bar plots.

### Temporal Analysis 📅
A temporal analysis is conducted to examine the distribution of penguin observations across different years. The counts of observations per year are visualized using a bar plot, allowing us to identify any trends or patterns over time.

### Variates across Categorical Variables 📈
We analyze variations in bill measurements and body mass across different species, genders, and islands. Average values of these variables are calculated and compared among categories to understand potential differences.

### Impact of Body Mass by Year, Gender, and Island 💪
We investigate the influence of year, gender, and island on body mass using statistical techniques such as ANOVA, Kruskal-Wallis H test, and Mann-Whitney U test. These tests help determine whether these factors independently impact body mass and whether there exists any interaction among them.

### Results and Interpretation 📝
- **Homogeneity of Variance:** While the variances of body mass across different years are homogeneous, they are not homogeneous across different genders or islands.
- **Normality:** The Shapiro-Wilk test indicates that the distribution of bill length does not follow a normal distribution.
- **ANOVA:** There is a significant difference in body mass across different islands and genders, but not across different years.
- **Kruskal-Wallis H Test:** There is a highly significant difference in body mass across different islands, indicating that the island of habitat significantly influences body mass. However, there is no significant difference across different years.
- **Mann-Whitney U Test:** The test results reveal a significant difference in body mass between male and female penguins.

### Conclusion 🎉
This EDA provides valuable insights into the distribution and patterns of penguin data. Variables such as species, island, and gender have a significant impact on body mass, while the year of observation does not. These findings can be further explored to understand the ecological and biological factors affecting penguin populations. Further analysis and modeling could be conducted to predict or classify penguin characteristics based on the identified patterns.
