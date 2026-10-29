# SpaceX Falcon 9 Landing Prediction

An IBM Data Science Professional Certificate capstone exploring historical launch data and first-stage landing outcomes.

## Workflow and notebook guide

| Stage | Material |
| --- | --- |
| Collection | [API notebook](Data%20Collection%20API.ipynb), [web scraping](Data%20Collection%20with%20Web%20Scraping.ipynb) |
| Preparation | [Data wrangling](Data%20Wrangling.ipynb) |
| Exploration | [SQL analysis](EDA%20with%20SQL.ipynb), [visual analysis](EDA%20with%20Data%20Visualization.ipynb) |
| Geography | [Folium notebook](Interactive%20Visual%20Analytics%20with%20Folium.ipynb) |
| Modelling | [Machine learning](Machine%20Learning%20Prediction.ipynb) |
| Communication | [Final presentation](DS-Capstone-Presentation.pdf), [saved plots](Plots/) |

An additional stock-data notebook is retained as separate coursework material.

## Explore locally

Install Python and Jupyter, then open the notebooks:

```bash
python -m pip install jupyter
jupyter notebook
```

Review each notebook's import/install cells and data paths before execution. A consolidated dependency file is not currently committed. External API and scraping steps may depend on network access and changes to their source services.

## Dashboard

[app.py](app.py) provides a Plotly Dash interface for launch-site outcomes and payload comparisons. It visualises historical records; it does not serve the trained landing classifier.

The script requires `spacex_launch_dash.csv`, which is **not included under that name**. Obtain the course dashboard dataset and verify its columns before running the app. Do not rename another CSV without checking its schema.

The dashboard also uses legacy Dash component imports and `run_server`; its dependency compatibility needs verification before a fresh installation can be considered reproducible.

## Interpretation

Model comparisons and plots document the coursework experiment. Their scope is the supplied historical data; they do not establish operational launch predictions.
