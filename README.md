# Global Food Inflation Dashboard (2001–2024)
![Dashboard Screenshot](https://github.com/Soph231/Food_inflation_visualization/blob/main/screenshots/Inflation_dashboard_screenshot_in_render.png)
An interactive dashboard for exploring global food inflation trends from 2001 to 2024. The application is built with Python and Dash and combines annual country-level inflation estimates with geographic data to provide interactive map and chart views.

Repository Structure
```
.
├── visual_Food_Inflation_app.py
├── requirements.txt
├── country_year_mean.csv
├── Inflation_data/
│   ├── Inflation_2001.geojson
│   ├── Inflation_2002.geojson
│   ├── ...
│   └── Inflation_2024.geojson
└── assets/
```
## Files
|File or Folder| Description|
|---|---|
|visual_Food_Inflation_app.py|	Main Dash application|
|requirements.txt|	Python package requirements|
|country_year_mean.csv|	Annual food inflation estimates by country|
|Inflation_data/|	GeoJSON files used to generate the map|
|assets/|	Images and styling resources used by Dash|

## Requirements
Install the required Python packages:

pip install -r requirements.txt

## Running the Dashboard

Clone the repository:

git clone https://github.com/your-username/your-repository.git
cd your-repository

Start the application:

python visual_Food_Inflation_app.py

Open your browser and navigate to:

http://127.0.0.1:8050/

## Data

The dashboard uses annual country-level food inflation estimates derived from monthly observations. GeoJSON files stored in the Inflation_data folder provide the geographical information required for the interactive map.

## Related Repository

A smaller reproducible example demonstrating the preprocessing workflow and a simplified dashboard is available in the [Mini Workflow Inflation Visualization repository](https://github.com/Soph231/Mini_workflow_Inflation_visualization). The mini version includes sample data and can be run locally, in Google Colab, or in Binder.

## Technologies
- Python
- Pandas
- Plotly
- Dash
- GeoJSON
- NumPy

## License
This repository is provided for educational and demonstration purposes.
