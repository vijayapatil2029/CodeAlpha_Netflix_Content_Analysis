# 🎬📊 Netflix Content Analysis

> **An exploratory data analysis project uncovering patterns, trends, and data-quality insights from Netflix Movies and TV Shows.**

---

## 📌 About The Project

Netflix Content Analysis is a data analytics project focused on exploring a dataset of Movies and TV Shows available on Netflix.

The project applies **data inspection, data-quality analysis, exploratory data analysis (EDA), statistical analysis, and visualization** to understand Netflix's content library.

The analysis explores content types, genres, ratings, countries, release years, movie durations, TV Show seasons, and Netflix content additions over time.

The project also identifies missing values, unusual records, duration outliers, and inconsistencies within the dataset.

---

## 🎯 Project Objectives

- 🧹 Examine and assess the quality of the Netflix dataset.
- 📊 Compare Movies and TV Shows.
- 🎭 Analyze genres, ratings, and content categories.
- 🌍 Explore the countries associated with Netflix content.
- 📅 Analyze release years and Netflix content addition trends.
- 🎬 Analyze movie durations and identify potential outliers.
- 📺 Analyze TV Show season distributions.
- 🔍 Investigate missing values and unusual records.
- 🧪 Compare Movie and TV Show release years using statistical analysis.
- 📈 Use visualizations to communicate important patterns and findings.

---

## 📂 Dataset

The project uses the **Netflix Movies and TV Shows** dataset.

### Dataset Details

| Attribute | Details |
|---|---|
| 📊 Records | 8,807 |
| 📋 Columns | 12 |
| 🎬 Content Types | Movies, TV Shows |
| 📄 Dataset File | `netflix_titles.csv` |

### Main Attributes

- `show_id`
- `type`
- `title`
- `director`
- `cast`
- `country`
- `date_added`
- `release_year`
- `rating`
- `duration`
- `listed_in`
- `description`

---

## 🧹 Data Quality Analysis

The dataset was examined for common data-quality issues.

### Checks Performed

- Missing-value analysis
- Duplicate-record detection
- Data-type inspection
- Invalid or unusual rating values
- Movie duration outlier analysis
- Release-to-Netflix time-lag analysis
- Negative time-lag detection

### Important Data Quality Findings

- Director information has a high proportion of missing values.
- Missing director information is particularly concentrated among TV Shows.
- Country and cast information also contain missing values.
- 98 records have missing or invalid `date_added` values after date conversion, all belonging to TV Shows.
- Four records have missing rating values.
- Values such as `66 min`, `74 min`, and `84 min` appear in the rating column and represent inconsistent data.
- Fourteen records have a negative release-to-Netflix time lag.
- No duplicate records were found.

---

## 🔍 Exploratory Data Analysis

The project explores the following areas:

### 🎬 Content Type Analysis

Comparison of Movies and TV Shows in the Netflix dataset.

### 🎭 Genre Analysis

Analysis of frequently occurring individual genre categories and genre diversity.

### ⭐ Rating Analysis

Analysis of Netflix content ratings and comparison of rating distributions between Movies and TV Shows.

### 🌍 Country Analysis

Analysis of countries associated with Netflix content and comparison of Movie and TV Show presence.

### 📅 Release Year Analysis

Analysis of content release years and comparison between Movies and TV Shows.

### ➕ Netflix Content Addition Trends

Analysis of the number of Movies and TV Shows added to Netflix over time.

### ⏱️ Movie Duration Analysis

Analysis of movie duration distribution, average duration, median duration, and potential outliers.

### 📺 TV Show Season Analysis

Analysis of the number of seasons across TV Shows.

### 🕐 Release-to-Netflix Lag Analysis

Comparison of the time between content release and its addition to Netflix.

---

## 📊 Key Insights

- Movies represent approximately **69.6%** of the dataset, while TV Shows represent approximately **30.4%**.
- Netflix content additions reached their highest total in **2019**, with 1,999 additions.
- **International Movies, Dramas, and Comedies** are among the most frequent individual genre categories.
- Approximately **67% of TV Shows have only one season**.
- Movie duration has a median of approximately **98 minutes**.
- Movie duration outliers include both legitimate short-form and long-form content.
- TV Shows have a more recent average release year than Movies.
- The average release year is approximately **2013.12 for Movies** and **2016.61 for TV Shows**.
- Missing director information is particularly concentrated among TV Shows.
- All **98 records with missing or invalid `date_added` values after date conversion are TV Shows**.

---

## 🧪 Statistical Analysis

A **Welch's t-test** was used to compare the release years of Movies and TV Shows.

### Results

| Metric | Value |
|---|---:|
| Average Movie Release Year | 2013.12 |
| Average TV Show Release Year | 2016.61 |
| p-value | 3.71 × 10⁻⁹⁵ |

The test found a statistically significant difference between the average release years of Movies and TV Shows.

This indicates that the two groups have different distributions of release years in the analyzed dataset.

---

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| 🐍 Python | Data analysis and processing |
| 🐼 Pandas | Data manipulation and analysis |
| 📊 Matplotlib | Data visualization |
| 🧪 SciPy | Statistical hypothesis testing |
| 📓 Jupyter Notebook | Analysis and documentation |
| 💻 VS Code | Development environment |

---

## 📁 Project Structure

```text
CodeAlpha_Netflix_Content_Analysis/
│
├── 📂 data/
│   └── netflix_titles.csv
│
├── 📓 netflix_analysis.ipynb
│
└── 📄 README.md

🔄 Project Workflow
Netflix Dataset
       ↓
Data Loading
       ↓
Data Inspection
       ↓
Data Quality Analysis
       ↓
Data Cleaning / Transformation
       ↓
Exploratory Data Analysis
       ↓
Statistical Analysis
       ↓
Data Visualization
       ↓
Key Findings
       ↓
Conclusion

💡 Project Outcomes

The project demonstrates how exploratory data analysis can be used to:

Understand a real-world dataset.
Identify patterns in Movies and TV Shows.
Analyze content trends over time.
Detect missing and inconsistent data.
Identify legitimate statistical outliers.
Compare groups using statistical testing.
Communicate findings through visualizations.
Convert raw data into meaningful insights.

🔮 Future Scope

Possible future improvements include:

🤖 Build a machine-learning model for Netflix content analysis.
📈 Develop predictive analysis for content trends.
🎯 Analyze audience-oriented content patterns.
🌍 Perform deeper country-level and regional analysis.
📊 Build an interactive dashboard using Streamlit or Power BI.
🔎 Perform more advanced statistical analysis.
☁️ Deploy an interactive analytics dashboard online.

📈 Project Status

🟢 Completed – Exploratory Data Analysis

Completed
✅ Dataset collection
✅ Dataset loading
✅ Data inspection
✅ Missing-value analysis
✅ Duplicate check
✅ Genre analysis
✅ Rating analysis
✅ Country analysis
✅ Release-year analysis
✅ Movie duration analysis
✅ TV Show season analysis
✅ Outlier analysis
✅ Statistical hypothesis testing
✅ Data visualization
✅ Key findings
✅ Project documentation
Future Improvements
⬜ Interactive dashboard
⬜ Advanced predictive analysis
⬜ Deployment
👤 Author

Vijaya Patil

B.Tech – Artificial Intelligence & Data Science

📜 License

This project is created for educational and internship purposes as part of the CodeAlpha Data Analytics Internship.

🎬 Netflix Content Analysis

Turning Netflix data into meaningful insights through exploratory data analysis.