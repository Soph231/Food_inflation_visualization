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

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Soph231/Food_inflation_visualization/blob/main/preprocessing_mini_sample/Inflation_data_preprocessing_pipeline_example.ipynb)

At the top of the notebook, install dependencies:
```python
!pip install -r requirements.txt

Option 2: Binder

Launch an interactive Jupyter session in your browser:
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/Soph231/Food_inflation_visualization/main?filepath=preprocessing_mini_sample%2FInflation_data_preprocessing_pipeline_example.ipynb)

### Option 3: Run Locally

You can also run the notebook on your own machine:

```bash
# Clone the full repository
git clone https://github.com/Soph231/Food_inflation_visualization.git

# Move into the mini sample subfolder
cd Food_inflation_visualization/preprocessing_mini_sample

# Install required dependencies
pip install -r requirements.txt

# Launch Jupyter Notebook
jupyter notebook Inflation_data_preprocessing_pipeline_example.ipynb
