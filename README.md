OLAP Demo – ROLAP, MOLAP, HOLAP in Python

Author : Whitney Gituara (ID: 528)

# OLAP-Operations-in-Python-ROLAP-MOLAP-HOLAP-Demo-
A practical Python demonstration of OLAP operations (ROLAP, MOLAP, HOLAP) with Pandas, SQLite, and visualizations.

📖 Overview

This repository demonstrates Online Analytical Processing (OLAP) concepts using Python.
OLAP is a technique for analyzing data from multiple perspectives, widely used in data warehousing and business intelligence.

The demo covers:

ROLAP (Relational OLAP): Using SQL queries on relational databases.

MOLAP (Multidimensional OLAP): Using in-memory data cubes (via Pandas pivot tables).

HOLAP (Hybrid OLAP): Combining relational and multidimensional approaches.

Visualizations are included for each method to help beginners understand how OLAP operations are applied in real-world scenarios.

📂 What’s Inside

olap_demo.ipynb / .py: Main script showing all OLAP operations.

SQLite database: Created dynamically from sample employee and department data.

Visualizations: Generated using Seaborn and Matplotlib.

⚙️ Features and Operations
🔹 ROLAP (Relational OLAP)

Runs SQL queries on a SQLite database.

Aggregates data such as average salary per department.

Example visualization: bar chart of department vs average salary.

🔹 MOLAP (Multidimensional OLAP)

Uses Pandas pivot tables to build in-memory cubes.

Slices data by department and age.

Example visualization: heatmap of salaries by department and age.

🔹 HOLAP (Hybrid OLAP)

Combines SQL queries (ROLAP) with Pandas aggregation (MOLAP).

Summarizes average salary per department.

Example visualization: grouped bar chart.

🔹 Core OLAP Functions

Slice: Filtering data (e.g., all employees in IT).

Dice: Filtering on multiple dimensions (e.g., HR employees with salary > 60,000).

Drill Down: Breaking down summary into detailed data.

Roll Up: Summarizing totals (e.g., total salary per department).

📊 Sample Outputs

ROLAP: Bar chart – Average Salary by Department.

MOLAP: Heatmap – Department vs Age cube.

HOLAP: Bar chart – Hybrid average salary summary.

OLAP Functions: Slicing, dicing, drill-down, roll-up with visual plots.

🛠️ Tools Used

Python – Main programming language.

Pandas & NumPy – Data manipulation and aggregation.

SQLite3 – Relational database for ROLAP queries.

Seaborn & Matplotlib – Data visualization.
