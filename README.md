````markdown
# IBM Data Science Capstone — SpaceX Falcon 9 Landing Prediction 🚀

This repository contains my work for the **IBM Data Science Professional Certificate Capstone**.  
The project follows an end-to-end data science workflow to analyze **SpaceX Falcon 9 launches** and build models to **predict whether the first stage will successfully land** (a key factor in reusability and launch cost).

---

## Project Goal

SpaceX can reduce launch costs by reusing the first stage.  
By predicting landing success using historical launch data, we can estimate mission risk and better understand what factors influence successful landings.

---

## What’s Inside

### ✅ Key Tasks Covered
- Data collection via **API**
- Data collection via **web scraping**
- Data cleaning & **wrangling**
- Exploratory data analysis (EDA) using:
  - **SQL**
  - **visual analytics**
- Interactive map-based analysis with **Folium**
- Machine learning classification to predict landing success
- Interactive dashboard using **Plotly Dash**

---

## Repository Structure

| File / Folder | Description |
|--------------|------------|
| `Data Collection API.ipynb` | Collect launch data using APIs |
| `Data Collection with Web Scraping.ipynb` | Scrape additional launch-related data from the web |
| `Data Wrangling.ipynb` | Clean, transform, and prepare datasets |
| `EDA with SQL.ipynb` | Explore the dataset using SQL queries |
| `EDA with Data Visualization.ipynb` | Visualize trends and insights using charts |
| `Interactive Visual Analytics with Folium.ipynb` | Geospatial analysis & interactive maps |
| `Machine Learning Prediction.ipynb` | Train/test ML models (classification) & compare performance |
| `app.py` | **Dash** app for interactive visualization |
| `DS-Capstone-Presentation.pdf` | Final presentation slides |
| `dataset_part_1.csv / dataset_part_2.csv / dataset_part_3.csv` | Processed datasets used across notebooks |
| `Spacex.csv`, `spacex_web_scraped.csv`, `spacex_launch_geo*.csv` | Additional dataset exports |
| `Plots/` | Saved plots/figures (if any) |

---

## Tools & Tech Stack

- **Python**
- **Pandas, NumPy**
- **Matplotlib, Seaborn**
- **SQL**
- **Folium**
- **scikit-learn**
- **Plotly, Dash**

---

## How to Run

### 1) Clone the repo
```bash
git clone https://github.com/hitesh175/IBM_Data_Science_Capstone.git
cd IBM_Data_Science_Capstone
````

### 2) (Recommended) Create a virtual environment

```bash
python -m venv .venv
# Windows
.venv\Scripts\activate
# macOS/Linux
source .venv/bin/activate
```

### 3) Install dependencies

```bash
pip install -r requirements.txt
```

> If you don’t have a `requirements.txt` yet, you can create one with:

```bash
pip freeze > requirements.txt
```

### 4) Run Jupyter notebooks

```bash
jupyter notebook
```

---

## Run the Dash Dashboard

The dashboard reads from `spacex_launch_dash.csv` and provides:

* Pie chart of landing success by launch site
* Scatter plot of landing success vs payload mass (filterable)

Run:

```bash
python app.py
```

Then open the local URL shown in your terminal (usually):

* [http://127.0.0.1:8050/](http://127.0.0.1:8050/)

---

## Machine Learning (High Level)

The ML notebook builds a pipeline to:

* Create the target label (`Class`) for landing success
* Standardize features
* Split into train/test
* Tune and compare multiple classifiers (via GridSearchCV), such as:

  * Logistic Regression
  * SVM
  * Decision Tree
  * KNN

---

## Results & Deliverables

* Cleaned datasets and EDA insights
* Interactive geospatial analysis (Folium)
* Predictive classification models
* Dash-based interactive dashboard
* Final PDF presentation

---

## Author

**Hitesh K R**
GitHub: [https://github.com/hitesh175](https://github.com/hitesh175)

---

## License

This project is for educational purposes as part of the IBM Data Science Professional Certificate.
(If you want, add a formal license like MIT by including a `LICENSE` file.)

```
::contentReference[oaicite:0]{index=0}
```
