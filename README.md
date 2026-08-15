# Processed E-commerce Dataset

## Project Overview

This project demonstrates e-commerce data preprocessing and integration using Python and Pandas. The three provided datasets — **Orders, Customers, and Products** — are loaded, combined, transformed, and exported as a final processed CSV dataset.

## Input Datasets

- `Day9_Orders.csv` — Order information
- `Day9_Customers.csv` — Customer information
- `Day9_Products.csv` — Product information

## What the Notebook Does

`Processed_Ecommerce_Dataset.ipynb` demonstrates:

1. Loading the three CSV files using Pandas.
2. Combining related information using `merge()`.
3. Demonstrating DataFrame combination using `concat()`.
4. Creating and transforming useful columns using `apply()`.
5. Converting order dates to DateTime format.
6. Extracting the month, day, weekday, and weekend information from the order date.
7. Creating calculated fields such as `Total_Amount` and quantity categories.
8. Organizing the result into a clean, meaningful DataFrame.
9. Exporting the final DataFrame as `Processed_Ecommerce_Dataset.csv`.

## How to Run the Project

### 1. Open the Notebook

Open `Processed_Ecommerce_Dataset.ipynb` in Google Colab or Jupyter Notebook.

### 2. Add the Input CSV Files

Upload these three files to the notebook's **Files** panel:

```text
Day9_Customers.csv
Day9_Orders.csv
Day9_Products.csv
```

Keep the filenames unchanged so that the notebook can locate them correctly.

### 3. Run the Notebook

Run the cells from top to bottom. The notebook displays intermediate results where applicable and performs the required merging, concatenation, transformations, and DateTime processing.

### 4. Generate the Processed Dataset

The final export cell creates the output file:

```python
output_file = "Processed_Ecommerce_Dataset.csv"
processed.to_csv(output_file, index=False)
```

After successful execution, the notebook confirms that the processed dataset has been exported.

### 5. Download the Output CSV

The notebook includes a final download cell:

```python
from google.colab import files
files.download("Processed_Ecommerce_Dataset.csv")
```

Run this cell after the export cell. Google Colab will download the generated `Processed_Ecommerce_Dataset.csv` file to your computer.

The downloaded CSV is the **final processed dataset** that should be submitted/uploaded along with the notebook.

## Repository Structure

```text
Processed_Ecommerce_Dataset/
│
├── Processed_Ecommerce_Dataset.ipynb
├── Processed_Ecommerce_Dataset.csv
├── Day9_Orders.csv
├── Day9_Customers.csv
├── Day9_Products.csv
└── README.md
```

## Tools Used

- Python
- Pandas
- Google Colab / Jupyter Notebook

## Output

The final `Processed_Ecommerce_Dataset.csv` contains integrated order, customer, and product information along with derived DateTime and analytical columns.

## GitHub Submission

Upload the following files to the GitHub repository:

- `Processed_Ecommerce_Dataset.ipynb`
- `Day9_Orders.csv`
- `Day9_Customers.csv`
- `Day9_Products.csv`
- `Processed_Ecommerce_Dataset.csv`
- `README.md`
