# ETL Midterm Project – Halima 315

## 1. Project Overview
This project demonstrates a complete ETL (Extract, Transform, Load) process using Python and Jupyter Notebook. It simulates the real-world scenario of working with both raw and incremental datasets, cleaning and transforming them, and loading them into structured formats like SQLite databases.

---

## 2. ETL Phases

- **etl_extract.ipynb**
  - Loads and previews `raw_data.csv` and `incremental_data.csv`
  - Displays `.head()` and `.info()` for initial inspection
  - Identifies missing values, duplicates, and unusual columns
  - Saves raw copies to the `data/` folder

- **etl_transform.ipynb**
  - Applies at least 4 key transformations, such as:
    - Removing duplicates
    - Handling missing values
    - Changing data types
    - Creating new calculated fields (e.g. `total_price`)
  - Saves cleaned datasets to:
    - `transformed_csv.csv`
    - `transformed_incremental.csv`

- **etl_load.ipynb**
  - Loads the transformed CSV files into SQLite databases
  - Uses SQL queries to preview the stored data
  - Output is saved in the `loaded/` folder as `.db` files

---

## 3. Tools Used

- Python 3.x  
- Jupyter Notebook  
- Pandas  
- SQLite (sqlite3)  
- Git & GitHub  
- (Optional) Parquet for file storage  
- (Optional) matplotlib or seaborn for visuals

---

## 4. How to Run the Project

1. **Clone the Repository**
   ```bash
   git clone https://github.com/halima-04/DSA2040A_ETL_Midterm_Halima_315.git
   cd DSA2040A_ETL_Midterm_Halima_315
