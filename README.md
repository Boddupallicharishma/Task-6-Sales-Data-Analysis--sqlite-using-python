📊 Sales Data Analysis

This project performs sales data analysis using SQL and Python. The analysis covers product-wise sales trends including total quantity sold and revenue generated.

📁 Project Structure
Edit
├── sales_data.db              # SQLite database containing sales records
├── sales_analysis.ipynb       # Jupyter notebook for SQL queries and visualization
├── sales_summary.py           # Python script to extract and summarize sales data
├── output/                    # Folder with CSV outputs and charts
└── README.md                  # Project documentation

🎯 Objectives
Analyze product-wise sales data.

Calculate total quantity sold per product.

Calculate total revenue generated per product.

Visualize the results using charts.

🛠️ Tools Used
Python 3.11

Pandas

SQLite3

Matplotlib / Seaborn (for visualization)

Jupyter Notebook / Google Colab

🧠 How It Works
Connects to the sales_data.db SQLite database.

Runs SQL queries like:

sql
Copy
Edit
SELECT 
    product,
    SUM(quantity) AS total_qty,
    SUM(quantity * price) AS revenue
FROM sales
GROUP BY product;
Results are loaded into a DataFrame and exported to a CSV file.

Charts are generated to visualize product performance.

📝 Usage
Clone the repo:

bash
Copy
Edit
git clone https://github.com/your-username/sales-data-analysis.git
cd sales-data-analysis
Install dependencies:

bash
Copy
Edit
pip install pandas matplotlib
Run the analysis:

Jupyter Notebook: sales_analysis.ipynb

Script: python sales_summary.py

View outputs in the output/ folder.

📦 Output
The output CSV contains:

Product	Total_Qty	Revenue
A	150	3000.0
B	120	2400.0

Visuals include bar charts for:

Quantity sold by product

Revenue by product

🧩 Troubleshooting
If you see no such table: sales, ensure the table exists by opening the database with a browser (like DB Browser for SQLite).

Make sure the table name and column names exactly match your query.

📬 Contact

Gmail: charishmaboddupalli@gmail.com
