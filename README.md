# Week 4 - Employee Data Analysis

A Python capstone project for Week 4. The project uses **Pandas** to read an employee CSV dataset, calculate the average salary, count employees by department, filter employees above a salary threshold, and export the filtered results to a new CSV file.

## Dataset

The included `data/employees.csv` is a small sample dataset so the project can be run immediately. If your instructor provided a specific Kaggle Employee Dataset, replace this CSV with that dataset and keep the required columns (`Name`, `Department`, `Salary`).

## Requirements

- Python 3.9+
- Pandas

## Project structure

```text
week4_employee_data_analysis/
├── data/
│   └── employees.csv
├── output/
│   └── employees_above_threshold.csv   # generated after running
├── employee_analysis.py
├── requirements.txt
├── .gitignore
└── README.md
```

## How to run

### 1. Create a virtual environment (recommended)

Windows:

```bash
python -m venv .venv
.venv\Scripts\activate
```

macOS/Linux:

```bash
python3 -m venv .venv
source .venv/bin/activate
```

### 2. Install the dependency

```bash
pip install -r requirements.txt
```

### 3. Run the analysis

```bash
python employee_analysis.py
```

The default salary threshold is **$70,000**.

To use a different threshold:

```bash
python employee_analysis.py --threshold 75000
```

To use a different CSV file or output location:

```bash
python employee_analysis.py --input data/employees.csv --threshold 70000 --output output/employees_above_threshold.csv
```

## Assignment requirements covered

- Load CSV using Pandas
- Calculate average salary
- Count employees by department
- Filter employees above a salary threshold
- Export filtered results to a new CSV

## Example result

After running the project, the filtered employees are saved in:

`output/employees_above_threshold.csv`
