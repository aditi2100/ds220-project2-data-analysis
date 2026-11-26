## 🎬Netflix Shows Data Analysis

**Course Project II – Data Analytics with Python (Pandas)**  
**Dataset:** Netflix Movies and TV Shows (Kaggle)

---

## 📊Overview

This project analyzes the **Netflix Movies and TV Shows** dataset from Kaggle.  
The goal is to explore global content trends, understand Netflix’s catalog growth, and identify patterns in genres, release years, countries, and availability over time.

The analysis was performed in **Python (Pandas)** using **Jupyter Notebook on GitHub Codespaces** and published using **GitHub Pages**.

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

## **Problem Space**
### **What?**  
This project analyzes Netflix’s global catalog of movies and TV shows using a structured data-driven approach. It examines patterns in content production, genre distribution, growth over time, and country-level contributions.

### **Why?**  
As streaming platforms continue to dominate the entertainment industry, understanding how Netflix curates and expands its catalog is essential. This analysis helps uncover trends in content availability, regional diversity, and viewing options. Such insights can guide strategic decisions, academic research, and discussions around global media consumption.

### **Who Benefits?**  
- Viewers seeking to understand available content and trends
- Media analysts examining streaming market behavior
- Entertainment industry professionals identifying production and distribution patterns
- Students & researchers analyzing real-world data for learning
- Content creators looking for opportunities based on genre and regional demand

### **Where & When?**  
The analysis uses Netflix’s internationally available dataset, containing titles released globally up to 2021. It reflects worldwide content trends rather than region-specific variations.

---

## **📜Questions to Address**
1. How many titles on Netflix are Movies vs TV Shows?  
2. How many titles were added each year?  
3. Which countries produce the most content?  
4. What are the most popular genres?  
5. How have release trends changed over time?  
6. Are Netflix titles single-genre or multi-genre?

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

- Netflix has more Movies than TV Shows, but TV content is rising. 
- Titles added to Netflix increased significantly between 2015–2020.  
- The United States and India are the largest contributors of Netflix content.  
- Dramas, International Movies, and Comedies are among the most common genres.
- Most titles belong to multiple genres, showing Netflix's multi-category classification style.   
- Release trends show a substantial increase in titles after 2010.  

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

This project demonstrates a complete data analysis workflow including importing external data, cleaning, transforming, EDA, visualization, insight generation, and publishing online using GitHub Pages.

The Netflix dataset provides valuable insights into global content distribution, production patterns, genre preferences, and evolving media trends.



