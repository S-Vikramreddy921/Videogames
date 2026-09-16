# Video Game Sales Analysis

A data analysis project exploring global video game sales, profit, and regional performance using Python, Pandas, Matplotlib, and Seaborn. The project cleans a raw video game sales dataset and visualizes trends across regions, countries, platforms, and genres.

## What This Project Does

**Data Cleaning**
- Removes duplicate records
- Fills missing values in the `Region` field
- Cleans and converts the `National Sales` column to numeric, filling missing values with the column average
- Standardizes country names (e.g., "USA" → "United States") and normalizes text formatting
- Caps extreme outliers in `National Sales` at the 95th percentile
- Renames columns for readability (`NA_Sales` → `National Sales`, `Global_Sales` → `Global Sales`, etc.)

**Visualizations**
- Bar chart — national sales by region and country
- Box plot — national sales by country, broken out by genre
- Pie charts — national vs. global sales share by country
- Line chart — national and global sales trends over time

## Tools & Libraries

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn

## Files in This Repo

- `VideoGamesYoutubeProject.ipynb` — the full analysis notebook
- `VideoGamesSales.csv` — the raw dataset used in the analysis

## Running It Locally

1. Clone the repo
2. Install dependencies: `pip install pandas numpy matplotlib seaborn`
3. Open `VideoGamesYoutubeProject.ipynb` in Jupyter Notebook or JupyterLab
4. Run all cells

> Note: the notebook currently loads the CSV from a local Windows path (`D:/Jupyter/VideoGamesSales.csv`). Since the CSV is now in this repo, update that line to `pd.read_csv('VideoGamesSales.csv')` so it runs for anyone who clones the project.
