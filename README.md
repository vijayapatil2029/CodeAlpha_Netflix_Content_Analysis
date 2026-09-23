# Netflix Content Analysis

## Project Overview

This project performs Exploratory Data Analysis (EDA) on a dataset of Netflix Movies and TV Shows.

The analysis explores the content available on Netflix and identifies patterns related to content type, genres, ratings, countries, release years, movie durations, TV Show seasons, and content additions over time.

The project also examines data-quality issues such as missing values, unusual records, and duration outliers, and uses statistical analysis to compare Movies and TV Shows.


## Project Objective

The main objectives of this project are to:

- Understand the structure and characteristics of the Netflix dataset.
- Compare Movies and TV Shows.
- Analyze genres, ratings, countries, release years, durations, and TV Show seasons.
- Identify trends in Netflix content additions over time.
- Detect missing values, unusual records, and potential data-quality issues.
- Use statistical analysis and visualizations to identify meaningful patterns.
- Summarize the major findings from the exploratory analysis.


## Dataset

The analysis uses the **Netflix Movies and TV Shows** dataset.

### Dataset Details

- **Rows:** 8,807
- **Columns:** 12
- **Content types:** Movies and TV Shows
- **Dataset file:** `netflix_titles.csv`

### Main Attributes

The dataset contains information about:

- Title
- Content type
- Director
- Cast
- Country
- Date added
- Release year
- Rating
- Duration
- Genre/category
- Description


## Tools & Technologies

- **Python**
- **Pandas** – Data manipulation and analysis
- **Matplotlib** – Data visualization
- **SciPy** – Statistical hypothesis testing
- **Jupyter Notebook** – Analysis and documentation
- **VS Code** – Development environment


## Analysis Performed

The project includes the following analyses:

- Dataset structure and data types
- Missing-value analysis
- Duplicate-record check
- Content-type distribution
- Rating analysis
- Country analysis
- Genre analysis
- Release-year analysis
- Netflix content addition trends
- Movie duration analysis
- Movie duration outlier analysis
- TV Show season analysis
- Release-to-Netflix time lag analysis
- Statistical comparison of Movie and TV Show release years
- Visual exploration of major patterns and trends


## Key Findings

- Movies represent approximately **69.6%** of the dataset, while TV Shows represent about **30.4%**.
- Netflix content additions increased strongly from 2016 onward and reached their highest level in **2019**.
- **International Movies, Dramas, and Comedies** are among the most frequent individual genre categories.
- Approximately **67% of TV Shows have only one season**.
- Movie durations are mainly concentrated around **80–120 minutes**, with a median of **98 minutes**.
- The identified movie duration outliers were found to represent legitimate short and long-form content.
- TV Shows have a **more recent average release year** than Movies.
- Missing director information is particularly concentrated among TV Shows.
- All **98 records with missing `date_added` values are TV Shows**.
- The analysis identified missing information in director, country, cast, date-added, and rating fields.


## Statistical Analysis

A Welch's t-test was used to compare the average release years of Movies and TV Shows.

The test found a statistically significant difference between the two groups, with TV Shows having a more recent average release year than Movies.

- **Average Movie release year:** 2013.12
- **Average TV Show release year:** 2016.61
- **p-value:** 3.71 × 10⁻⁹⁵


## Data Quality Notes

The dataset contains several data-quality issues that were identified during the analysis:

- Missing values are present in `director`, `country`, `cast`, `date_added`, and `rating`.
- Director information is missing for a large proportion of TV Shows.
- Four records have missing rating values.
- Some rating values such as `66 min`, `74 min`, and `84 min` appear to be incorrectly placed duration values.
- Fourteen records have a negative release-to-Netflix time lag, indicating possible inconsistencies in the source data.
- No duplicate records were found.