# 🧪 ETL Midterm Project – Halima (ID: 315)

## 📌 Project Overview

This ETL (Extract, Transform, Load) mini-project showcases the entire ETL pipeline applied to two datasets: `raw_data.csv` and `incremental_data.csv`. The goal is to extract raw data, apply meaningful transformations, and load the cleaned and structured results into SQLite databases — a process that mirrors real-world data engineering and analytics workflows.

The project is organized into three separate notebooks:
- `etl_extract.ipynb` – Extracts and inspects raw data
- `etl_transform.ipynb` – Applies data cleaning and transformations
- `etl_load.ipynb` – Loads transformed data into SQLite databases

---

## 🗂️ Project Folder Structure
ETL_Midterm_Halima_315/
├── data/
│ ├── raw_data.csv
│ └── incremental_data.csv
├── transformed/
│ ├── transformed_full.csv
│ └── transformed_incremental.csv
├── loaded/
│ ├── full_data.db
│ └── incremental_data.db
├── screenshots/
│ ├── extract_preview.png
│ ├── transform_changes.png
│ └── load_query.png
├── etl_extract.ipynb
├── etl_transform.ipynb
├── etl_load.ipynb
├── README.md
└── .gitignore


## 🔁 ETL Phase Breakdown

### 1. 📥 Extract – `etl_extract.ipynb`
- Loaded both `raw_data.csv` and `incremental_data.csv` using pandas
- Displayed `.head()` and `.info()` for both datasets
- Noted important observations such as:
  - Missing values
  - Duplicate rows
  - Inconsistent data types
- Saved clean copies in the `data/` folder for version control

### 2. 🔧 Transform – `etl_transform.ipynb`
At least 4 meaningful transformations were applied:

| Category        | Description                                                                 |
|----------------|-----------------------------------------------------------------------------|
| 🧹 Cleaning      | Removed duplicate rows using `.drop_duplicates()`                          |
| ❓ Handling NA   | Filled or removed missing values with defaults or statistical values       |
| 🧮 Enrichment    | Added a new column `total_price = quantity * unit_price`                   |
| 🗓️ Structural    | Converted date columns to datetime format using `pd.to_datetime()`         |
| 🧑‍🎓 Categorization | Created age bins with `pd.cut()` to group customers into age segments     |

**Before and after** transformations were displayed with markdown explanations.

### 3. 🗃️ Load – `etl_load.ipynb`
- Loaded the transformed datasets into SQLite databases using `sqlite3`
- Stored results in `loaded/` folder as:
  - `full_data.db`
  - `incremental_data.db`
- Previewed stored tables using SQL query:
  
🛠 Tools Used
Tool	Purpose
Python 3.12	Core programming language
Jupyter Notebook	Interface for running ETL code
Pandas	Data loading and transformation
SQLite3	Lightweight database engine
Git & GitHub	Version control and online repository
VS Code / Terminal	Code editing and Git CLI usage

🚀 How to Run the Project
📁 Clone the Repository
bash
Copy
Edit
git clone https://github.com/halima-04/DSA2040A_ETL_Midterm_Halima_315.git
cd DSA2040A_ETL_Midterm_Halima_315
📓 Open Jupyter Notebooks
Run the notebooks in this order:

etl_extract.ipynb

etl_transform.ipynb

etl_load.ipynb

🔍 Explore Outputs
Transformed CSVs → transformed/

SQLite DB files → loaded/

Screenshots → screenshots/

🖼️ Screenshots
Extract Phase	Transform Phase	Load Phase

