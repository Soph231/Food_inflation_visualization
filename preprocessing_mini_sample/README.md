# Mini Inflation Data Preprocessing Sample

This folder contains a **mini, end-to-end demo** of the data preprocessing pipeline used in the Inflation Dashboard.  
It uses a small synthetic dataset (Australia & New Zealand, 2001–2002) so the notebook can run quickly and reproducibly on GitHub, Colab, or Binder.

---

## 📂 Folder Structure
<pre>'''preprocessing_mini_sample/
├─ data_raw/
│ ├─ sample_data.csv # sample monthly data (2 countries × 2 years × 12 months each)
│ └─ custom.geo.json # minimal GeoJSON (AUS + NZ polygons)

├─ sample_data/ # output folder created by the notebook
│ ├─ country-year_mean.csv
│ ├─ Inflation_2001.geojson
│ └─ Inflation_2002.geojson

├─ Inflation_data_preprocessing_pipeline_example.ipynb # notebook (data prep, EDA plots, Folium map)
├─ requirements.txt # Python dependencies
└─ README.md # this file'''<pre>

## How to Run

###  Option 1: Google Colab
Open directly in Colab:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/<YOUR_USERNAME>/<YOUR_REPO>/blob/main/preprocessing_mini_sample/Inflation_data_preprocessing_pipeline_example.ipynb)

At the top of the notebook, install dependencies:
```python
!pip install -r requirements.txt

Option 2: Binder

Launch an interactive Jupyter session in your browser:
https://mybinder.org/v2/gh/soawesomedigital/Inflation_Dashboard/main?filepath=preprocessing_mini_sample%2FInflation_data_preprocessing_pipeline_example.ipynb

Option 3: Run Locally

Clone the repo and run the notebook:
git clone https://github.com/<YOUR_USERNAME>/<YOUR_REPO>.git
cd <YOUR_REPO>/preprocessing_mini_sample
pip install -r requirements.txt
jupyter notebook Inflation_data_preprocessing_pipeline_example.ipynb
