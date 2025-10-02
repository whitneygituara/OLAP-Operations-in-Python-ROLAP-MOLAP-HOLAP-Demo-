OLAP Demo – ROLAP, MOLAP, HOLAP in Python
Author
Whitney Gituara (ID: 528)
________________________________________
📖 What is OLAP?
Online Analytical Processing (OLAP) is a category of software tools that allow users to analyze large datasets quickly and interactively.
Unlike OLTP (Online Transaction Processing) systems, which handle day-to-day operations (e.g., banking systems, sales transactions), OLAP focuses on analysis and decision-making.
Think of OLAP as a way to answer questions like:
•	“What’s the average salary per department?”
•	“Which age group earns the most in Engineering?”
•	“How do sales this year compare to last year, broken down by region?”
________________________________________
🛠️Why this project?
If you are new to Data Warehousing or OLAP concepts, this notebook provides a beginner-friendly, hands-on introduction. You will see how relational databases and multidimensional cubes work together for analytical processing.
________________________________________
🔑 Key OLAP Concepts
1. ROLAP (Relational OLAP)
•	Works directly on relational databases (like SQL, SQLite, MySQL).
•	Uses SQL queries to calculate aggregates (SUM, AVG, COUNT, etc.).
•	Pros: Handles very large datasets.
•	Cons: Querying can be slower than MOLAP.
👉 In this demo:
We calculate the average salary per department using SQL queries on SQLite.
________________________________________
2. MOLAP (Multidimensional OLAP)
•	Stores data in cubes (multidimensional arrays).
•	Works in-memory, making it fast for complex aggregations.
•	Pros: Fast querying once the cube is built.
•	Cons: Requires enough memory, less scalable for very large datasets.
👉 In this demo:
We build a salary cube with dimensions:
•	Rows = Department
•	Columns = Age
•	Values = Average salary
This lets us see salaries from multiple perspectives at once.
________________________________________
3. HOLAP (Hybrid OLAP)
•	Combines ROLAP and MOLAP approaches.
•	Stores detailed data in relational databases but pre-computes summaries in cubes.
•	Pros: Balanced speed and scalability.
•	Cons: More complex to implement.
👉 In this demo:
We fetch detailed data using SQL (ROLAP) and then use Pandas to build summaries (MOLAP).
________________________________________
4
.OLAP Operations (The "4 Pillars")
Operation	Meaning	Example in Demo
Slice	Take one dimension and look at just one value
	Salaries of all employees in IT department
Dice	Take a smaller cube by filtering on multiple dimensions
	Employees in HR earning > 60,000
Drill Down	Go from summarized data to detailed data	
Average salary → Individual salaries by employee
Roll Up	Aggregate detailed data into higher-level summaries	Total salary per department

________________________________________
📂 What’s Inside the Repository
•	olap_demo.ipynb – Jupyter Notebook with full code and explanations.
•	olap_demo.db – SQLite database automatically created with employees & departments data.
•	Visualizations – Bar charts and heatmaps to show results of OLAP operations.
________________________________________
📊 Sample Visuals You’ll See
1.	ROLAP – Bar chart of average salary per department.
2.	MOLAP – Heatmap of department vs age (average salaries).
3.	HOLAP – Bar chart of hybrid average salaries.
4.	Roll Up – Total salary per department.
________________________________________
🛠️ Tools Used
•	Python – Main programming language.
•	Pandas & NumPy – For MOLAP and HOLAP aggregation.
•	SQLite3 – Relational database backend (ROLAP).
•	Seaborn & Matplotlib – Visualizations.
________________________________________
How to Run the Demo	
1.	Clone the repository:
2.	git clone https://github.com/whitneygituara/OLAP-Demo.git
3.	cd OLAP-Demo
4.	Install dependencies:
5.	pip install pandas numpy matplotlib seaborn
6.	Run the Jupyter notebook:
7.	jupyter notebook olap_demo.ipynb
________________________________________
🎯 Learning Outcomes
By the end of this demo, you will:
✅ Understand what OLAP is and why it’s important in data warehousing.
✅ See the difference between ROLAP, MOLAP, and HOLAP.
✅ Learn how to apply slice, dice, drill-down, and roll-up operations.
✅ Be able to use SQL + Pandas to simulate OLAP in Python.


