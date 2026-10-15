# Analyze Forest Fire Incidence by Region and Season

A course-end project for **Exploratory Data Analysis and Visualization (EDAV) – 22AC31N**, Department of Information Technology, Chaitanya Bharathi Institute of Technology, Hyderabad.

**Team:** *(add names and roll numbers)*

## What this project does

We take monthly forest fire records for 62 forest regions across 6 continents and answer five questions with Python:

| # | Question | Bloom's level |
|---|----------|---------------|
| Q1 | Calculate average fire incidence | 3 |
| Q2 | Filter fire data by region | 3 |
| Q3 | Handle missing fire records | 4 |
| Q4 | Group fire incidences by season and region | 4 |
| Q5 | Visualize fire frequency trends | 5 |

## A note on the data

The dataset's `Data_Type` column says **"SIMULATED / EDUCATIONAL – not observed fire records"**. The results show how the analysis works. They are not real-world fire statistics.

## Files

- `forest_fire_analysis.ipynb` – the Google Colab notebook with all the code, logic and conclusions
- `forest_fire_analysis.py` – the same code as a plain Python file (explanations are comments)
- `Forest_Fire_Project.pptx` – the project presentation
- `Forest_Fire_Project.pdf` – the presentation as a PDF
- `images/` – charts produced by the notebook
- `forest_fire_dataset_one_sheet.xlsx` – the dataset (add it to the repo next to the notebook)

## How to run

1. Open `forest_fire_analysis.ipynb` in [Google Colab](https://colab.research.google.com/) (File → Upload notebook, or open it straight from GitHub).
2. Upload `forest_fire_dataset_one_sheet.xlsx` to the Colab files panel. It lands in `/content/`, which is the path the notebook reads from.
3. Run the cells from top to bottom.

Running locally instead? Install `numpy pandas matplotlib seaborn openpyxl`, then change `/content/` in the file paths to your own folder.

## Tools used

Python 3, NumPy, Pandas, Matplotlib, Seaborn.

## What we found

- About **26.6 fires per region per month** on average.
- **Summer** (43.9) and the tropical **dry season** (42.8) are the busiest; winter (10.0) is the quietest.
- **43 of 62 regions** peak in summer.
- Adding all regions together gives a fairly flat line, because the northern and southern hemispheres peak in opposite months. The seasonal pattern shows up clearly only when the data is split by continent.
- The 7 missing records were filled with the median of the same region's other months.

## Charts

![Matplotlib subplots](images/fire_trends_matplotlib.png)
![Seaborn subplots](images/fire_trends_seaborn.png)
![Continent facets](images/fire_trends_facetgrid.png)
