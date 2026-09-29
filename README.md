# DataAnalyzer

**DataAnalyzer** is an interactive Python tool for loading, exploring, cleaning, analyzing, and visualizing datasets. It provides a user-friendly menu-driven interface for handling common data tasks without writing custom code.

---

## Features

1. **Load Dataset**
   - Load CSV files into a Pandas DataFrame.
   - Automatically converts data to a NumPy array for further analysis.

2. **Explore Data**
   - View first or last rows.
   - Display column names and data types.
   - Get a summary of the dataset using `info()`.

3. **Clean & Handle Missing Data**
   - Remove duplicate rows.
   - Drop rows with excessive missing values.
   - Fill missing numeric values with column mean.
   - Fill missing categorical values with `"Unknown"`.

4. **DataFrame Operations**
   - Convert DataFrame to NumPy arrays (with indexing and slicing options).
   - Perform arithmetic operations (add, subtract, multiply, divide) between columns.
   - Calculate percentages or aggregate functions (sum, mean).
   - Combine multiple datasets.
   - Split dataset by column values.
   - Search, sort, and filter data.

5. **Descriptive Statistics**
   - Compute standard deviation, variance, and quantiles.
   - Aggregate functions: sum, mean, count.
   - Create pivot tables.

6. **Data Visualization**
   - Bar Plot
   - Box Plot
   - Scatter Plot
   - Histogram
   - Heatmap
   - Pie Chart
   - Stack Plot
   - Save visualizations as image files.

---

## Installation

1. Clone the repository or download the script.
2. Install dependencies using pip:

```bash
pip install pandas numpy matplotlib seaborn
```

3. Run the main script:

```bash
python data_analyzer.py
```

---

## Usage

- The program is menu-driven. Simply follow the prompts to load datasets, explore, clean, analyze, and visualize your data.
- Example workflow:
  1. Load a CSV dataset.
  2. Explore the dataset to check structure and missing values.
  3. Clean the data to handle duplicates and missing entries.
  4. Perform operations like combining datasets or adding calculated columns.
  5. Generate statistics and pivot tables for insights.
  6. Visualize the data with various chart types.
  7. Save your plots for reporting.

---

## Notes

- Works with numeric and categorical data.
- Handles missing values intelligently for both numeric and categorical columns.
- Visualizations use Seaborn and Matplotlib for high-quality plots.
- Supports large datasets efficiently using Pandas and NumPy.

---

## Example

```python
from data_analyzer import DataAnalyzer

analyzer = DataAnalyzer("sales_data.csv")
analyzer.explore()
analyzer.clean_data()
analyzer.mathematical_operations()
analyzer.visualize_data()
analyzer.save_visualization()
```

---

## License

This project is open-source and free to use.
