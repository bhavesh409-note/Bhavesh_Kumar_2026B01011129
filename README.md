# Employee Data Cleaning with Pandas

**Name:** Bhavesh Kumar
**Roll No:** 2026B01011129
**Course:** Data Analyst

A beginner-friendly Google Colab notebook that explores and cleans a messy employee dataset using only **pandas**.

## Files

| File | Description |
|------|-------------|
| `Bhavesh_Kumar_2026B01011129_Data_Analyst.ipynb` | Main notebook with all the code |
| `employee_data_messy.csv` | Raw dataset (103 rows, 9 columns) with intentionally messy data |

## Dataset Issues

The raw data contains typical real-world problems:

- Inconsistent text case and extra spaces (e.g. `HR` / `hr`, `Mumbai` / `MUMBAI` / `Jaipur `)
- Missing values in `Age`, `Salary`, `Email` and `Rating`
- Impossible ages (negative and 250)
- `Salary` stored as text (e.g. `Rs. 93000`)
- Mixed date formats in `Join_Date`
- Fully duplicated rows

## What the Notebook Covers

**1. Loading the data**
- `pd.read_csv()`

**2. Exploring the data**
- `head()`, `tail()`, `sample()`
- `shape`, `columns`, `dtypes`, `info()`
- `describe()` and `describe(include='all')`
- `value_counts()` and `unique()`
- `isna().sum()` and `duplicated().sum()`

**3. Selecting data**
- Column selection: `df['Age']`
- Row selection with `loc` and `iloc`

**4. Cleaning the data**
- Checking `mean()`, `median()` and `mode()` to choose a fill value
- Filling missing values with `fillna()`
- Dropping columns with `drop(columns=[...])`
- Removing duplicate rows with `drop_duplicates()`
- Changing data types with `astype()`

## How to Run

1. Open [Google Colab](https://colab.research.google.com) and choose **File → Upload notebook**.
2. Select `Bhavesh_Kumar_2026B01011129_Data_Analyst.ipynb`.
3. Run the first cell and upload `employee_data_messy.csv` when prompted.
4. Run the remaining cells in order.

## Tools Used

- Python 3
- pandas
- Google Colab
