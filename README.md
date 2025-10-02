# 📊 OLAP Demo – ROLAP, MOLAP, HOLAP in Python

### 👩‍💻 Author

Whitney Gituara (ID: 528)

---

## 📖 What is OLAP?

**Online Analytical Processing (OLAP)** is a category of tools that allow users to analyze large datasets quickly and interactively.

🔹 Unlike **OLTP (Online Transaction Processing)** systems, which handle day-to-day operations (e.g., banking, sales), OLAP focuses on **analysis and decision-making**.

Think of OLAP as a way to answer questions like:

* *“What’s the average salary per department?”*
* *“Which age group earns the most in Engineering?”*
* *“How do sales this year compare to last year, broken down by region?”*

---

## 🛠️ Why this Project?

If you are new to **Data Warehousing** or **OLAP**, this notebook provides a **beginner-friendly, hands-on introduction**.
You will see how:

* Relational databases (ROLAP)
* Multidimensional cubes (MOLAP)
* Hybrid approaches (HOLAP)

work together for analytical processing.

---

## 🔑 Key OLAP Concepts

### 1️⃣ ROLAP (Relational OLAP)

* Works directly on **relational databases** (SQLite, MySQL, PostgreSQL).
* Uses **SQL queries** for aggregation (`SUM`, `AVG`, `COUNT`).
* ✅ **Pros**: Handles very large datasets.
* ❌ **Cons**: Can be slower than MOLAP.

👉 *In this demo:* We calculate **average salary per department** using SQL queries in SQLite.

---

### 2️⃣ MOLAP (Multidimensional OLAP)

* Stores data in **cubes** (multidimensional arrays).
* Performs **fast in-memory calculations**.
* ✅ **Pros**: Very fast once cube is built.
* ❌ **Cons**: Needs memory, less scalable for massive datasets.

👉 *In this demo:* We build a cube with:

* **Rows** = Department
* **Columns** = Age
* **Values** = Average Salary

---

### 3️⃣ HOLAP (Hybrid OLAP)

* Combines **ROLAP + MOLAP**.
* Detailed data stays in the relational database, but summaries are pre-computed in cubes.
* ✅ **Pros**: Balanced speed & scalability.
* ❌ **Cons**: More complex.

👉 *In this demo:* We fetch detailed salary data using SQL (**ROLAP**) and summarize it in Pandas (**MOLAP**).

---

### 4️⃣ OLAP Operations (The Four Pillars)

| Operation      | Meaning                             | Example in Demo                       |
| -------------- | ----------------------------------- | ------------------------------------- |
| **Slice**      | Fix one dimension                   | Salaries of employees in **IT**       |
| **Dice**       | Filter on multiple dimensions       | Employees in **HR** earning > 60,000  |
| **Drill Down** | From summary → details              | Dept avg salary → individual salaries |
| **Roll Up**    | Aggregate into higher-level summary | Total salary **per department**       |

---

## 📂 Repository Contents

* `OLAP operations.ipynb` → Jupyter Notebook with code & explanations
* `olap_demo.db` → SQLite database (auto-generated)
* Visualizations → Bar charts & heatmaps showing OLAP operations

---

## 📊 Visuals You’ll See

1. 📉 **ROLAP** – Avg Salary per Department (bar chart)
2. 🔥 **MOLAP** – Dept vs Age Salary Cube (heatmap)
3. 📊 **HOLAP** – Hybrid Avg Salaries (bar chart)
4. 📈 **Roll Up** – Total Salary per Department

---

## 🛠️ Tools & Libraries

* **Python** → main language
* **Pandas & NumPy** → data processing + MOLAP
* **SQLite3** → relational backend (ROLAP)
* **Seaborn & Matplotlib** → data visualization

---

## 🚀 How to Run the Demo

```bash
# 1. Clone the repository
git clone https://github.com/whitneygituara/OLAP-Operations-in-Python-ROLAP-MOLAP-HOLAP-Demo-.git
cd OLAP-Operations-in-Python-ROLAP-MOLAP-HOLAP-Demo-

# 2. Install dependencies
pip install pandas numpy matplotlib seaborn

# 3. Run the notebook
jupyter notebook "OLAP operations.ipynb"
```

---

## 🎯 Learning Outcomes

By the end of this demo, you will:
✅ Understand **what OLAP is** and why it matters in Data Warehousing
✅ Compare **ROLAP, MOLAP, and HOLAP**
✅ Apply **slice, dice, drill-down, and roll-up** operations
✅ Use **SQL + Pandas** to simulate OLAP in Python

