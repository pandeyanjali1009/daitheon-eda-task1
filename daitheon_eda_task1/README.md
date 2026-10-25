# Daitheon Internship — EDA Task 1: Superstore Sales

## Objective
Explore sales volume, monthly seasonality, category performance, region/customer-segment performance, and discount sensitivity.

## Project structure
```text
daitheon_eda_task1/
├── data/
│   └── superstore_sales.csv
├── outputs/                  # created when the notebook runs
├── eda_superstore_sales.ipynb
├── requirements.txt
├── .gitignore
└── README.md
```

## Run in Cursor (Windows PowerShell)
1. Open this project folder in Cursor.
2. Open Terminal → New Terminal.
3. Create a virtual environment:
   ```powershell
   py -m venv .venv
   ```
4. Activate it:
   ```powershell
   .\.venv\Scripts\Activate.ps1
   ```
   If PowerShell blocks activation, use:
   ```powershell
   Set-ExecutionPolicy -Scope Process -ExecutionPolicy Bypass
   .\.venv\Scripts\Activate.ps1
   ```
5. Install dependencies:
   ```powershell
   python -m pip install --upgrade pip
   pip install -r requirements.txt
   ```
6. In Cursor, open `eda_superstore_sales.ipynb`. Select the `.venv` Python interpreter/kernel if prompted.
7. Click **Run All**. Check that all charts, summary tables, takeaways, and exported CSV files appear.

## Data cleaning note
The supplied CSV contains rows without essential order/date/sales fields. The notebook reports missing values and removes rows that cannot support the analysis. It does not invent missing postal codes.

## Git commands
From the project root:
```powershell
git init
git add README.md requirements.txt eda_superstore_sales.ipynb data/superstore_sales.csv .gitignore
git commit -m "Complete Superstore sales EDA task"
```
Create an empty repository on your Git hosting site, then connect it using the repository URL shown by that site:
```powershell
git branch -M main
git remote add origin YOUR_REPOSITORY_URL
git push -u origin main
```
Replace `YOUR_REPOSITORY_URL` with your actual repository URL. Never commit passwords, API keys, or private credentials.
