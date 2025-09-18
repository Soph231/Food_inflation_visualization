# Visual Food Inflation – Sample Dash App  

This folder contains a minimal **Dash application** that demonstrates how to visualize the processed sample inflation data produced by the preprocessing pipeline.  

## Folder Structure  
preprocessing_mini_sample/
├─ sample_data/ # Output files created by the preprocessing pipeline
│ ├─ country-year_mean.csv
│ ├─ Inflation_2001.geojson
│ └─ Inflation_2002.geojson
│
├─ app/
│ ├─ app.py # Dash application
│ ├─ requirements.txt # Dependencies for running the app
│ └─ README.md # This file

## ️ Running the App  

1. **Install dependencies**  

   From inside the `app/` folder (or repo root if you prefer a global requirements file):  

   ```bash
   pip install -r requirements.txt
2. **Run the app**
```bash
python sample_app.py
The app will start a local server (default http://127.0.0.1:8050/).
Open this link in your browser to interact with the dashboard.
3. ***Default behavior***
The app automatically scans ../sample_data/ for available Inflation_*.geojson files.

A year dropdown is populated dynamically.

By default, the most recent year (e.g., 2002 in this sample dataset) is displayed.
##Notes
This sample uses a very small dataset (AUS and NZ for 2001–2002).

For full-scale usage, generate yearly GeoJSON files and CSV summaries with the preprocessing pipeline notebook (Inflation_data_preprocessing_pipeline_example.ipynb).

The app code is path-relative, so it will continue to work if this folder is renamed (e.g., from preprocessing_mini_sample/ → sample_pipeline/).


