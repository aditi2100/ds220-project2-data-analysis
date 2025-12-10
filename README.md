## 🎬Netflix Shows Data Analysis

**Course Project II – Data Analytics with Python (Pandas)**  
**Dataset:** Netflix Movies and TV Shows (Kaggle)

---

## 📊Overview

This project presents a comprehensive data analysis of the Netflix Movies and TV Shows dataset sourced from Kaggle. The objective is to explore global content trends on Netflix, understand the evolution of its catalog, and identify meaningful patterns related to genres, countries, release years, content types, and availability over time.

The project follows a complete data workflow—from acquisition and cleaning to exploratory analysis, visualization, and insight generation—implemented in Python, Pandas, and Jupyter Notebook within GitHub Codespaces. The final deliverable is published through GitHub Pages, as required by the project specifications.

---

## 🎯Project Objectives

This project aims to:

- Perform structured data cleaning and preprocessing
- Conduct exploratory data analysis (EDA) using Pandas
- Create meaningful visualizations using Matplotlib and Seaborn
- Answer targeted analytical questions based on the dataset
- Present a clear narrative linking insights to the broader problem space
- Publish a reproducible analysis notebook using GitHub Pages

---

## 📂Dataset Description

**Dataset Name:** Netflix Movies and TV Shows  
**Source:** [Kaggle](https://www.kaggle.com/datasets/shivamb/netflix-shows)  
**File Used:** `netflix_titles.csv`  
**Record Count:** ~8,800 titles  

**Main Columns Include:**

- `type` — Movie or TV Show
- `title` — Title name
- `director` — Director(s)
- `cast` — Main cast
- `country` — Production country
- `date_added` — Date added to Netflix
- `release_year` — Original release year
- `duration` — Runtime (Movies) or number of seasons (TV Shows)
- `listed_in` — Categories/genres
- `description` — Brief summary

---

## 📜Questions Addressed

- How many titles on Netflix are Movies vs TV Shows?
- How many titles were added to Netflix each year?
- Which countries produce the most Netflix content?
- What are the most popular genres on Netflix?
- How has the number of releases changed over time?
- Are Netflix titles primarily single-genre or multi-genre?

---

## 🫧Data Cleaning Performed

Key preprocessing steps included:

- Converting `date_added` into datetime format  
- Extracting `added_year` and `added_month`  
- Handling missing values in `country`, `director`, and `listed_in`  
- Splitting multi-genre fields  
- Parsing and converting `duration` values  
- Creating a `num_genres` feature  
- Standardizing column names (lowercase, underscore format)  

---

## ⚙️Techniques & Tools Used

- Python 3  
- Pandas  
- NumPy  
- Matplotlib and Seaborn  
- Jupyter Notebook (Codespaces)  
- GitHub for version control  
- GitHub Pages for final project publication  

---

## Project Structure

**project/**  
- **data/**  
  - raw/ → Raw dataset files (ZIP and CSV)  
  - processed/ → Cleaned data (optional)  
- **notebooks/**  
  - netflix_analysis.ipynb → Main analysis notebook  
- **docs/**  
  - index.html → Exported HTML for GitHub Pages  
- README.md → Project documentation  
- requirements.txt → Python dependencies  

---

## GitHub Pages Publication

The final notebook is exported as an HTML file and published using GitHub Pages.

**Final GitHub Pages URL:**  
https://aditi2100.github.io/ds220-project2-data-analysis/docs/  

---

## ✅Key Insights

- Netflix contains more Movies than TV Shows, though TV content has grown in recent years.  
- Titles added to Netflix increased significantly between 2015–2020.  
- The United States and India are the largest contributors of Netflix content.  
- Dramas, International Movies, and Comedies are among the most common genres.  
- Release trends show a substantial increase in titles after 2010.  
- Most titles belong to multiple genres, showing Netflix's multi-category classification style.  

---

## How to Run This Project (in Codespaces)

1. Open the repository in GitHub Codespaces.  
2. Upload your Kaggle ZIP file into the `data/raw/` directory.  

3. Use the following code inside your notebook to extract and load the dataset:

```python
!unzip "../data/raw/netflix-shows.zip" -d "../data/raw/"
import pandas as pd
df = pd.read_csv("../data/raw/netflix_titles.csv")
````

4. Run all cells in the notebook.
5. Export the notebook to HTML:

```bash
jupyter nbconvert --to html notebooks/netflix_analysis.ipynb --output ../docs/index.html
```

6. Enable GitHub Pages using the `/docs` folder.

---

## ✍️Author

**Aditi Pawar**  
Course: Data Science (DS220)  
Semester: Fall 2025  

---

## ✅Conclusion

This project demonstrates the complete workflow of data analysis—from importing external data, preprocessing and transforming it, conducting exploratory analysis, answering well-defined questions, and publishing the final results online.

The Netflix dataset provides valuable insights into global content distribution, international production patterns, genre preferences, and shifting media trends over time.




