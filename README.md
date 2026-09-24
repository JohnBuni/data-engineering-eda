# Data Engineering & EDA Workshop

This project demonstrates an end-to-end data engineering and exploratory data analysis (EDA) workflow using Python, PostgreSQL, Pandas, and Jupyter Notebook.

The project generates a synthetic employee dataset, stores the data in a PostgreSQL database, retrieves it into Python for analysis, and performs data cleaning, transformation, statistical analysis, feature engineering, and visualization.

## Project Workflow

The notebook demonstrates:

- Synthetic employee data generation using Faker
- Object-oriented programming (OOP) for organizing the workflow
- PostgreSQL database storage and retrieval
- Database connectivity using psycopg2
- Data cleaning and transformation with Pandas
- Descriptive statistical analysis
- Feature engineering
- Salary standardization
- Dataset merging
- Data visualization with Matplotlib and Seaborn
- Grouped analysis and heatmap visualization

## Project Structure

```text
data-engineering-eda/
│
├── notebooks/
│   └── .gitkeep
│
├── prompts/
│   └── .gitkeep
│
├── src/
│   └── .gitkeep
│
├── data_engineering_eda.ipynb
├── requirements.txt
├── .gitignore
└── README.md
```

The `notebooks`, `prompts`, and `src` directories are included as part of the project structure and are currently empty.

The `.env` file required for the database connection is not stored in this GitHub repository. It will be provided separately.

## Requirements

Before running the project, make sure you have:

- Python 3 installed
- Git installed
- Visual Studio Code
- Jupyter support in VS Code
- The provided `.env` file containing the required PostgreSQL database connection information

## How to Download and Run the Project

### 1. Clone the Repository

Open PowerShell or the VS Code terminal and run:

```powershell
git clone https://github.com/JohnBuni/data-engineering-eda.git
```

Move into the repository:

```powershell
cd data-engineering-eda
```

### 2. Open the Project in VS Code

From the repository folder, run:

```powershell
code .
```

Alternatively, open Visual Studio Code, select **File → Open Folder**, and select the `data-engineering-eda` folder.

### 3. Create a Virtual Environment

In the VS Code terminal, run:

```powershell
python -m venv .venv
```

This creates an isolated Python environment for the project.

### 4. Activate the Virtual Environment

On Windows PowerShell, run:

```powershell
.\.venv\Scripts\Activate.ps1
```

After activation, the terminal should display `(.venv)` at the beginning of the command prompt.

### 5. Install the Required Python Packages

Run:

```powershell
python -m pip install -r requirements.txt
```

This installs the Python libraries required to run the project.

### 6. Add the Provided `.env` File

The `.env` file containing the required PostgreSQL database connection information will be provided separately.

Place the provided `.env` file in the root directory of the cloned repository:

```text
data-engineering-eda/
│
├── notebooks/
├── prompts/
├── src/
├── .env
├── data_engineering_eda.ipynb
├── requirements.txt
├── .gitignore
└── README.md
```

Do not rename or modify the `.env` file unless instructed to do so.

The `.env` file is excluded from GitHub because it contains private database credentials.

### 7. Open the Jupyter Notebook

Open:

```text
data_engineering_eda.ipynb
```

in Visual Studio Code.

When prompted to select a Jupyter kernel, select the Python interpreter from the project's `.venv` environment.

You can verify that the notebook is using the correct Python environment by running:

```python
import sys
print(sys.executable)
```

The displayed path should point to the project's virtual environment, similar to:

```text
data-engineering-eda\.venv\Scripts\python.exe
```

### 8. Run the Notebook

In VS Code, select:

**Restart Kernel → Run All**

Run the notebook from top to bottom so that data generation, database operations, analysis, and visualizations execute in the intended order.

## Dataset

The primary employee dataset used in this project is generated programmatically using the Python Faker library rather than downloaded as a static external dataset.

The generated dataset contains employee information used throughout the database and exploratory data analysis workflow.

## Technologies

- Python
- Jupyter Notebook
- PostgreSQL
- Pandas
- NumPy
- Faker
- psycopg2
- scikit-learn
- Matplotlib
- Seaborn

## Security

The `.env` file containing the PostgreSQL database credentials is intentionally excluded from this GitHub repository for security.

For assignment submission, the required `.env` file will be provided separately in the submitted ZIP folder under the subject line **"9115726 - Data Engineering & EDA Workshop"**.

Database credentials and other sensitive configuration information should never be committed to the GitHub repository.