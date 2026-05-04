# Pandas & Matplotlib Exercises

A collection of hands-on Python exercises exploring data manipulation with **Pandas** and data visualization with **Matplotlib**, using a real-world dataset of data science job postings.

---

## Dataset

**Source:** [`lukebarousse/data_jobs`](https://huggingface.co/datasets/lukebarousse/data_jobs) (loaded via Hugging Face `datasets` library)

The dataset contains information on data-related job postings including job titles, locations, countries, posting dates, and salary figures.

---

## Topics Covered

### 1. NumPy Fundamentals
- Generating large random datasets and computing statistics (`mean`, `median`)
- Performance comparison between the `statistics` module and NumPy
- Array operations: creating arrays, element-wise multiplication
- Applied salary calculation using base salaries and bonus rates for data roles

### 2. Data Loading & Exploration
- Loading a Hugging Face dataset and converting it to a Pandas DataFrame
- Previewing data with `.head()`, inspecting structure with `.info()` and `.describe()`
- Filtering rows using conditional expressions (e.g. job title, salary threshold)
- Exploring unique values with `.unique()`

### 3. Data Cleaning
- Converting date columns to `datetime` format using `pd.to_datetime()`
- Sorting the DataFrame by date with `.sort_values()`
- Dropping unnecessary columns with `.drop()`
- Removing rows with missing salary values using `.dropna()`

### 4. Data Analysis
- Identifying minimum salary entries using `.idxmin()` and `.iloc[]`
- Grouping data by job title to compute mean, median, min, max, and count of salaries
- Multi-level grouping by job title and country
- Filtering for US-specific jobs and aggregating salary statistics

### 5. Time Series Analysis
- Extracting the month from datetime columns
- Counting and sorting monthly job postings
- Plotting monthly posting trends as a line chart

### 6. Data Visualization with Matplotlib
- **Line chart** — sine wave plot to demonstrate basic plotting
- **Line chart** — monthly job posting trends over the year
- **Horizontal bar chart** — count of job postings by job title (sorted ascending)
- **Vertical bar chart** — job postings per title with rotated labels
- **Scatter plot** — salary over time (job posted date vs. average yearly salary)
- **Resampled line chart** — monthly median salary trend
- **Histogram** — distribution of average yearly salaries with custom `$K` axis formatting
- **Horizontal bar chart** — median salary by job title (sorted)

---

## Libraries Used

| Library | Purpose |
|---|---|
| `numpy` | Array operations and numerical computing |
| `pandas` | Data manipulation and analysis |
| `matplotlib` | Data visualization |
| `datasets` | Loading the Hugging Face job postings dataset |
| `itables` | Interactive table display in notebooks |
| `statistics` | Built-in Python statistics (used for comparison) |

---

## How to Run

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/your-repo-name.git
   cd your-repo-name
   ```

2. **Install dependencies**
   ```bash
   pip install pandas numpy matplotlib datasets itables
   ```

3. **Run the script**
   ```bash
   python copy_of_pandas_lesson.py
   ```

   > **Note:** This script was originally developed in Google Colab. For the best experience, open it as a Jupyter/Colab notebook.

---

## Key Takeaways

- NumPy is significantly faster than Python's built-in `statistics` module for large datasets
- Pandas makes it straightforward to clean, filter, group, and aggregate real-world data
- Matplotlib offers flexible chart types for communicating data insights clearly
- Resampling time series data (e.g. monthly median) smooths out noise and reveals trends
