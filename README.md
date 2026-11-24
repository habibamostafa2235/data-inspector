# Data Inspector

A lightweight Python notebook for inspecting and summarizing tabular datasets (`.csv`, `.xlsx`, `.xls`). It validates file paths, loads data safely, and prints a structured overview of rows, columns, missing values, and sample records.

## Features
- **File & Format Validation:** Verifies that the path exists, points to a file, and uses a supported extension (`.csv`, `.xlsx`, `.xls`).
- **Safe Data Loading:** Supports CSV files (with UTF-8 and Latin-1 fallback) and Excel files, with error handling for empty or unreadable files.
- **Dataset Summary:** Displays total rows, columns, duplicate rows, transposed first 5 rows, and a per-column breakdown of data types, missing counts/percentages, and unique values.
- **Flexible Path Input:** Accepts a file path directly via `run_inspector(file_path)` or prompts interactively when left as `None`.

## Installation
```bash
pip install -r requirements.txt
## Installation

```bash
pip install -r requirements.txt
```

## Usage

Open `automation_data.ipynb` in Jupyter Notebook or VS Code and run the cells. You can pass a file path directly:

```python
df = run_inspector("path/to/your/file.xlsx")
```

Or call `run_inspector()` with no arguments to be prompted for a path.
