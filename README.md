## TMDb Movies Dataset Analysis

### Introduction

Welcome to the Exploratory Data Analysis for the TMDb Movie Dataset! This script delves into the diverse world of movies, utilizing the extensive information provided in the dataset, which includes details about 10,000 movies collected from The Movie Database (TMDb). The dataset spans a range of features, from user ratings and revenue to genres and cast information.

### Table of Contents
- [Data Wrangling](#wrangling)
- [Exploratory Data Analysis](#eda)
- [Conclusions](#conclusions)

### Data Wrangling

#### Observation from the Dataset

1. 9 columns have missing values in the entries.
2. Currency in revenue and budget columns does not have a unit specified to differentiate from other sets of numbers.
3. Release date is a datetime type but it is structured as a string.
4. Only one duplicate is seen in the dataset.

#### Data Cleaning

- Removed unnecessary columns.
- Converted the release date column from string to date format.
- Removed duplicate values.
- Replaced zero with NaN in the runtime column.
- Replaced all values from '0' to NaN in 'budget' and 'revenue' columns, then removed them.
- Changed the format of budget and revenue columns.

### Exploratory Data Analysis

#### Research Question 1 - Which movies had the highest and lowest budgets?

- Movie with ID 2244 shows the highest budget of $425,000,000.
- Movie with ID 2618 shows the lowest budget of $1.

#### Research Question 2 - Which movies had the highest and lowest revenue?

- Movie with ID 1386 (Avatar) shows the highest revenue of $2,781,505,847.
- Movie with ID 5067 shows the lowest revenue of $2.

#### Research Question 3 - Which movies had the highest and lowest profit?

- Movie with ID 1386 (Avatar) shows the highest profit of $2,544,505,847.
- Movie with ID 2244 shows the lowest profit of -$413,912,431.

#### Research Question 4 - Which movies had the longest and shortest runtime, and how does it relate to revenue?

- Movie with ID 2107 shows the longest runtime of 338 minutes.
- Movie with ID 5162 shows the shortest runtime of 15 minutes.

#### Research Question 5 - What kinds of properties are associated with movies that have high revenues?

- Average Budget: $60 million
- Average Revenue: $255 million
- Average Duration: 113 minutes
- Most Frequent Cast: Tom Cruise, Brad Pitt, Tom Hanks, Sylvester Stallone, Cameron Diaz
- Successful Genres: Action, Adventure, Thriller, Comedy, Drama

#### Research Question 6 - What is the average runtime of the movies?

- The average runtime of the movies is approximately 109.22 minutes.

#### Research Question 8 - Which year had the most profitable movies?

- The most profitable year was 2015 with a total profit of $19,032,145,273.

#### Research Question 9 - Which genres are most popular from year to year?

- The analysis provides a dynamic view of audience preferences and industry trends for different genres over the years.

### Conclusions

1. **Revenue and Budget Distribution:**
   - The distribution of movie revenue is right-skewed, indicating that a few movies generate significantly higher revenue than the majority.
   - Movie budgets also exhibit a right-skewed distribution, with most movies having relatively lower budgets.

2. **Genre Trends:**
   - The most prevalent movie genres include Drama, Comedy, and Action.
   - Genre popularity has evolved over the years, with certain genres gaining or losing prominence.

3. **Cast and Revenue:**
   - Certain actors and actresses appear more frequently in the dataset, suggesting potential star power.
   - Further analysis is needed to explore the correlation between specific cast members and high movie revenue.

4. **Budget and Revenue Relationship:**
   - A positive correlation exists between movie budgets and revenue, indicating that higher-budget movies tend to generate more revenue.
   - However, other factors may influence revenue, and a more detailed analysis is required.

5. **Profit Analysis:**
    - Movie with ID 1386 shows the highest earned profit i.e $254,450,5847.
    - Movie with ID 2244 shows the lowest earned profit i.e -$413,912,431.

6. **Most Profitable Year:**
    - The most profitable year was 2015 with a total profit of $19,032,145,273.00.

7. **Genre Popularity Over Time:**
    - The analysis of genre popularity over the years provides a dynamic view of audience preferences and industry trends.

**Recommendations:**
- Consider exploring more advanced machine learning models for revenue prediction.
- Conduct deeper analysis on outlier movies to understand their impact on overall trends.
- Investigate the influence of specific cast members and directors on movie success.
- Stay updated on evolving genre preferences and market dynamics for strategic decision-making in the film industry.
