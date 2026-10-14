# 🎬 Movie Market Analysis

### Data Analytics Case Study | Movie Ratings, Genre Performance & Box-Office Revenue

## 📌 Project Overview

Movie Market Analysis is a Python-based data analytics project that explores movie ratings, genre-level performance, box-office revenue, and highly rated films.

Using a dataset of 20 movies, this project applies data analysis and visualization techniques to identify patterns in audience ratings, compare genres, understand revenue distribution, and classify movies with IMDb ratings of 8.0 or above.

The project demonstrates practical skills in data manipulation, statistical summaries, exploratory data analysis, and visualization using Python.

## 🎯 Project Objectives

- Calculate the average IMDb rating across all movies.
- Compare average IMDb ratings across genres.
- Analyze total box-office revenue by genre.
- Visualize the distribution of IMDb ratings.
- Identify hit movies using an IMDb rating threshold of 8.0.
- Summarize key findings and provide data-driven interpretations.

## 🗂️ Project Structure

```text
movie-market-analysis/
│
├── README.md
├── Movie_Market_Analysis.ipynb
├── movie_ratings_dataset.csv
└── movie_market_analysis_report.pdf
```

## 📁 Dataset Description

The dataset contains **20 movie records** and five original columns.

| Column | Description |
|---|---|
| `Movie_ID` | Unique movie identifier |
| `Genre` | Movie genre: Action, Comedy, Drama, or Thriller |
| `Duration_Minutes` | Movie runtime in minutes |
| `IMDB_Rating` | IMDb rating recorded in the dataset |
| `Box_Office_Millions` | Box-office revenue, expressed in millions |

A derived `Hit` column is created during analysis to identify movies with ratings of 8.0 or higher.

## 🛠️ Technologies Used

- **Python** — Programming language
- **Pandas** — Data manipulation and analysis
- **Matplotlib** — Data visualization
- **Jupyter Notebook** — Interactive analysis
- **Google Colab** — Cloud-based notebook execution

## ⚙️ Analysis Workflow

### 1. Data Loading and Exploration

Load the CSV dataset into a Pandas DataFrame and inspect its structure, records, and columns.

### 2. Average IMDb Rating

Calculate the mean IMDb rating to understand the overall rating level in the sample.

### 3. Genre-Wise Rating Analysis

Group movies by genre and calculate the average IMDb rating and movie count for each genre.

### 4. Financial Impact Analysis

Aggregate box-office revenue by genre to compare total revenue across the four genres.

### 5. Rating Distribution

Create a histogram to examine the distribution of movie ratings and identify rating ranges with more movies.

### 6. Hit Movie Identification

Classify movies using the following rule:

```python
movies["Hit"] = movies["IMDB_Rating"] >= 8
```

Movies with ratings of 8.0 or above are classified as hits.

### 7. Hit Movie Summary

Calculate the total number and percentage of hit movies and examine their genre distribution.

## 📊 Key Findings

The following findings are taken from the accompanying analysis report.

### Overall Rating

- **Total movies analyzed:** 20
- **Average IMDb rating:** 7.21 out of 10

### Average IMDb Rating by Genre

| Genre | Average Rating | Movie Count |
|---|---:|---:|
| Thriller | 7.53 | 7 |
| Action | 7.50 | 5 |
| Comedy | 7.23 | 3 |
| Drama | 6.46 | 5 |

**Key observation:** Thriller has the highest average IMDb rating at 7.53, narrowly exceeding Action at 7.50.

### Total Box-Office Revenue by Genre

| Genre | Total Revenue (Millions) | Movie Count |
|---|---:|---:|
| Thriller | 1,777.2 | 7 |
| Action | 1,383.8 | 5 |
| Drama | 1,339.9 | 5 |
| Comedy | 1,076.1 | 3 |

**Key observation:** Thriller has the highest total box-office revenue in the supplied dataset.

These are aggregate revenue figures, not measures of individual movie profitability. Genres with more movies may naturally accumulate higher total revenue.

### IMDb Rating Distribution

The report groups ratings into the following bands:

| IMDb Rating Band | Number of Movies |
|---|---:|
| 5.0–5.9 | 3 |
| 6.0–6.9 | 6 |
| 7.0–7.9 | 6 |
| 8.0–8.9 | 2 |
| 9.0–9.9 | 3 |

**Key observation:** Twelve of the 20 movies (60%) fall within the 6.0–7.9 rating range.

### Hit Movie Analysis

- **Hit threshold:** IMDb rating greater than or equal to 8.0
- **Total hit movies:** 5
- **Percentage of hit movies:** 25%
- **Thriller:** 3 hit movies
- **Action:** 1 hit movie
- **Comedy:** 1 hit movie
- **Drama:** 0 hit movies

The highest-rated movie is `Movie_ID 4004`, a Comedy movie rated 9.5. The highest individual box-office revenue belongs to `Movie_ID 4010`, a Thriller movie with revenue of 486.9 million.

This demonstrates that the highest-rated movie is not necessarily the highest-grossing movie.

## 💡 Key Insights and Recommendations

1. **Study the Thriller genre:** It leads the sample in average IMDb rating, total revenue, and number of hit movies.
2. **Evaluate Action movies:** Action has an average rating close to Thriller and substantial total revenue.
3. **Investigate Drama ratings:** Drama has the lowest average rating in the sample, suggesting an opportunity for further analysis.
4. **Explore rating and revenue relationships:** Analyze whether higher ratings are associated with greater box-office revenue at the individual movie level.
5. **Expand the dataset:** Include more movies, release years, budgets, and marketing costs to better understand performance and profitability.

## 🚀 How to Run the Project

### Option 1: Google Colab

1. Open [Google Colab](https://colab.research.google.com/).
2. Upload `Movie_Market_Analysis.ipynb`.
3. Upload `movie_ratings_dataset.csv` when required.
4. Run the notebook cells sequentially.
5. Review the output tables, charts, and findings.

### Option 2: Run Locally

**Step 1: Clone the repository**

```bash
git clone https://github.com/YOUR_USERNAME/movie-market-analysis.git
```

**Step 2: Navigate to the project folder**

```bash
cd movie-market-analysis
```

**Step 3: Install the required libraries**

```bash
pip install pandas matplotlib jupyter
```

**Step 4: Launch Jupyter Notebook**

```bash
jupyter notebook
```

Open `Movie_Market_Analysis.ipynb` and execute the cells.

**Note:** Ensure that the notebook loads `movie_ratings_dataset.csv` from the project directory using `pd.read_csv()`. Update any dataset-loading cell that refers to a different filename or file format.

## 📄 Project Report

The `movie_market_analysis_report.pdf` file contains the detailed case study, including:

- Introduction and dataset description.
- Average IMDb rating calculation.
- Genre-wise rating comparisons.
- Box-office revenue analysis.
- Rating distribution visualization.
- Hit movie identification.
- Key findings and conclusion.

## ⚠️ Limitations

- The dataset contains only 20 movies.
- The findings describe the supplied sample and may not represent the broader movie market.
- Total box-office revenue does not account for production budgets, marketing costs, or profit margins.
- Additional variables are required to investigate factors influencing ratings and commercial performance.
- Observed patterns should not be interpreted as causal relationships.

## 🏁 Conclusion

The analysis identifies Thriller as the strongest-performing genre under the selected measures in this sample, with the highest average IMDb rating, total box-office revenue, and number of hit movies.

Five of the 20 movies meet the defined hit threshold, while most ratings fall between 6.0 and 7.9. Further analysis using a larger dataset and additional financial and movie attributes could provide deeper insights into audience preferences and commercial performance.

## 👨‍💻 Author

**Abhinandan Babu Munnoli**

Aspiring AI & Machine Learning Engineer | Python Developer | Final-Year Computer Science Engineering Student

- **GitHub:** [Abhi-munnoli](https://github.com/Abhi-munnoli)
- **LinkedIn:** [Connect with me](https://www.linkedin.com/in/abhinandan-munnoli-361a932bb/)

---

⭐ If you find this project useful, consider giving the repository a star.

*Developed as a data analytics case study for educational purposes.*
