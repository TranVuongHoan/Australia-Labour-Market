# Data Preparation

## Data Examination

In the initial phase of the project, I examined the original data files, which were provided in Excel format. Below is a summary of the fields contained in each dataset:

---

### **1. 6202005 (1).xlsx**

This file contains three sheets — **Index**, **Data1**, and **Enquiries** — representing survey and response data for the SOPS 2020 dataset.

#### **Index**
Contains metadata and explanations for variable codes used in the main data file.

- `Variable name` – Short code used in the dataset.  
- `Label` – Full description of the variable.  
- `Type` – Variable type (categorical, numeric, etc.).  
- `Values` – Response categories or coded values.  

#### **Data1**
Represents the main survey data containing participant responses and attributes.

- `Respondent_ID` – Unique identifier for each respondent.  
- `Institution` – Name or code of the institution.  
- `Division` – Faculty or department classification.  
- `Gender`, `Age`, `Years_in_role` – Demographic information.  
- Multiple columns representing survey question responses, using coded variables defined in the *Index* sheet.  

#### **Enquiries**
Contains metadata and reference information for handling queries or documentation related to the SOPS dataset.

---

### **2. SOPS-2024-Remuneration.xlsx**

This file contains four sheets providing remuneration breakdowns across industries, occupations, and classifications.

#### **By industry**
- `Industry` – Industry sector name.  
- `Average_salary`, `Median_salary` – Key pay metrics.  
- `Change_from_2023` – Year-over-year variation.  

#### **By key occupations in entities**
- `Occupation` – Specific job title or functional role.  
- `Entity_type` – Type of employing organisation.  
- `Mean_remuneration`, `Sample_size`.  

#### **By VPS grade classification**
- `Classification` – VPS grade level.  
- `Average_salary`, `Min_salary`, `Max_salary`.  
- `Change_from_previous_year`.  

#### **By VPS occupations**
- `Occupation` – Position title.  
- `Average_salary`, `Median_salary`.  
- `Entity_type`, `Sample_size`.  

---

## Data Transformation

To prepare the data for analysis and integration between the 2020 and 2024 datasets, I performed the following transformation steps:

1. **Standardize variable names**  
   - Converted inconsistent naming conventions to lowercase and replaced spaces with underscores.  
   - Example: `Average Salary` → `average_salary`.  

2. **Create unique identifiers**  
   - Added ID columns for institutions, divisions, and occupations to facilitate joins across datasets.  

3. **Map coded values to labels**  
   - Used the `Index` sheet in *6202005 (1).xlsx* to replace coded responses in `Data1` with full descriptive labels.  

4. **Handle missing values**  
   - Replaced blanks and “n/a” with standardized nulls (`NaN`) for numeric consistency.  

5. **Validate consistency between datasets**  
   - Cross-checked overlapping categories (e.g., industries and occupations) between the 2020 and 2024 data to ensure naming alignment.  

6. **Export transformed data**  
   - Saved cleaned and standardized files as CSV in a `modified_files/` directory.  

---

## Data Transformation Tools and Outputs

The data transformation process was automated using a Python Jupyter Notebook (`csv_files_preparation.ipynb`).  

Key libraries used:  
- **pandas** – for data cleaning, transformation, and merging  
- **numpy** – for handling missing data  
- **openpyxl** – for Excel I/O  

The final cleaned and standardized datasets are stored in the following directories:


