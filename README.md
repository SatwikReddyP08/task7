# Task 7: Sales Summary from SQLite Database

## Objective
The goal was to use Python to query a small SQLite database, summarize sales data (quantity and revenue), and create a bar chart, as per Elevate Labs' Task 7.

---

## Dataset Used
- **sales_data.db**: A SQLite database with one table (`sales`), containing 10 rows:
  - `product`: Product name (e.g., Laptop, Phone)
  - `quantity`: Units sold
  - `price`: Unit price

---

## Tools Used
- **Python**: For scripting (`sqlite3`, `pandas`, `matplotlib`)
- **SQLite**: File-based database
- **Google Colab**: For running code and generating outputs

---

## Approach
1. **Database Creation**:
   - Created `sales_data.db` using `sqlite3` in Colab.
   - Added a `sales` table with 10 rows of sample data.
2. **SQL Queries**:
   - Query 1: Summarized total quantity and revenue by product using `GROUP BY`.
   - Query 2: Calculated overall quantity and revenue.
3. **Output**:
   - Printed results as tables using `pandas`.
   - Generated a bar chart of revenue by product using `matplotlib`.

---

## Files
- `task_7_sales_summary.py`: Colab notebook with all code (database, queries, chart).
- `data/sales_data.db`: SQLite database file.
- `screenshots/sales_chart.png`: Bar chart showing revenue by product.
- `README.md`: This file.

---

## How to Run
1. Clone this repository.
2. Open `task_7_sales_summary.ipynb` in Google Colab.
3. Install dependencies (run the first cell: `pip install pandas matplotlib`).
4. Run all cells to see tables, chart, and download files.
5. Check `sales_chart.png` for the visualization.

---

## Learnings
- **SQLite**: Learned to create and query a database using `sqlite3.connect`.
- **SQL**: Got comfortable with `SUM`, `GROUP BY`, and calculating revenue (`quantity * price`).
- **Pandas**: Used DataFrames to display query results cleanly.
- **Matplotlib**: Created and saved a bar chart, adjusted labels.
- **Debugging**: Fixed a `CREATE TABLE` syntax error by adding quotes.
- **Colab**: Mastered downloading files and exporting notebooks.

---

## Insights
- Laptops ($2999.97) and Phones ($2499.95) generated the highest revenue due to high prices.
- Mice had the most units sold (16) but lowest revenue ($319.84) due to low price.
- Total sales: 37 units, $8039.63 revenue.

---

## Author
Satwik Reddy Pathapati
