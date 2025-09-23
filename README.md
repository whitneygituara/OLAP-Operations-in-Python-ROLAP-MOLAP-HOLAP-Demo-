# Simple Data Warehouse using Python, Pandas, and SQLite3 🗄️

This project demonstrates how to create a **simple data warehouse** in Python using:

- **SQLite3** for database management  
- **Pandas** for data manipulation  
- **Matplotlib / Seaborn** for visualization  

The script connects to a SQLite database, creates tables from a DataFrame, performs basic data analysis, and generates visualizations.

---

## 🧾 Features

The code includes the following functionality:

- ✅ Create a database connection (SQLite)  
- ✅ Execute SQL queries  
- ✅ Fetch and display data from tables  
- ✅ Convert Pandas DataFrames into database tables  
- ✅ Perform **basic data analysis** (head, info, describe, missing values)  
- ✅ Visualize data using **bar, line, or scatter plots**  

---

## 📂 Repository Contents

- `Day-1.ipynb` — Jupyter Notebook version of the project  
- `data_warehouse.db` — SQLite database file (created when running the script)  
- `main.py` — Python script (if you extract the code into a `.py` file)  

---

## ⚙️ Requirements

This project requires Python 3.8+ and the following libraries:

- `pandas`
- `sqlite3` (built-in with Python)
- `matplotlib`
- `seaborn`
- `numpy`
- `datetime` (built-in with Python)

You can install external dependencies with:

```bash
pip install pandas matplotlib seaborn numpy

pip install -r requirements.txt
