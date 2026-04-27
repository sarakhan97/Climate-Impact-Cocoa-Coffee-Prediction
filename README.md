# ClimaSense: Coffee and Cocoa Prediction Models

This repository contains Jupyter Notebook experiments for predicting cocoa and coffee quality/yield using climate and crop-related data.

## Project folders

```text
climasense_project_ready/
├── cocoa/
│   ├── 01_cocoa_yield_prediction.ipynb
│   ├── 02_cocoa_quality_prediction.ipynb
│   ├── 03_cocoa_tabnet_quality_experiments.ipynb
│   ├── archive_cocoa_first_experiments.ipynb
│   ├── Climate_dataset.csv
│   ├── UNdata_Cleaned_Yield-2.csv
│   └── full_flavors_of_cocoa_cleaned-2.csv
├── coffee/
│   ├── clean_coffee_2008.ipynb
│   ├── clean_coffee_data_2023.ipynb
│   ├── clean_coffee_data_2025.ipynb
│   ├── coffee_combined_clean.ipynb
│   ├── random_forest.ipynb
│   ├── xgboost.ipynb
│   ├── LSTM.ipynb
│   ├── Wrapper.ipynb
│   └── resnet.ipynb
├── requirements.txt
└── .gitignore
```

## How to run in Jupyter Notebook

### 1. Create and activate an environment

```bash
python3 -m venv .venv
source .venv/bin/activate
```

For Windows:

```bash
python -m venv .venv
.venv\Scripts\activate
```

### 2. Install packages

```bash
pip install -r requirements.txt
```

If `pytorch-tabnet` or `tensorflow` fails on your system, install the rest first and then install those packages separately.

### 3. Start Jupyter

```bash
jupyter notebook
```

### 4. Recommended running order

For cocoa:

1. `cocoa/01_cocoa_yield_prediction.ipynb`
2. `cocoa/02_cocoa_quality_prediction.ipynb`
3. `cocoa/03_cocoa_tabnet_quality_experiments.ipynb`

Note: `03_cocoa_tabnet_quality_experiments.ipynb` expects `final_quality_dataset.csv`, which is created by `02_cocoa_quality_prediction.ipynb`.

For coffee:

1. Add the missing coffee CSV files listed below.
2. Run cleaning notebooks first:
   - `clean_coffee_2008.ipynb`
   - `clean_coffee_data_2023.ipynb`
   - `clean_coffee_data_2025.ipynb`
   - `coffee_combined_clean.ipynb`
3. Run model notebooks:
   - `random_forest.ipynb`
   - `xgboost.ipynb`
   - `LSTM.ipynb`
   - `Wrapper.ipynb`
   - `resnet.ipynb`

## Missing coffee data files

The uploaded Coffee ZIP contains notebooks only. These notebooks reference CSV files that were not included in the ZIP:

- `arabica_2008.csv`
- `arabica_clean_2023.csv`
- `arabica-2024-25.csv`
- `cleaned_Coffee_Data.csv`
- `removed_outliners.csv`
- `final_coffee.csv`
- `final_coffee_no_area_year.csv`

Add these files to the `coffee/` folder before running the coffee notebooks.

## GitHub upload commands

```bash
git init
git add .
git commit -m "Initial commit: coffee and cocoa prediction notebooks"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/YOUR-REPO-NAME.git
git push -u origin main
```

Replace `YOUR-USERNAME` and `YOUR-REPO-NAME` with your GitHub username and repository name.

## Notes

Generated model files, temporary outputs, and large files are ignored through `.gitignore`.


## Run order
See `RUN_ORDER.md` for the recommended notebook execution order and missing coffee data files.
