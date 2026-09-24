# Data Engineering & EDA Workshop

This project demonstrates an end-to-end data engineering and exploratory data analysis (EDA) workflow using Python, PostgreSQL, Pandas, and Jupyter Notebook.

The project generates a synthetic employee dataset, stores the data in a PostgreSQL database, retrieves it for analysis, and performs data cleaning, transformation, statistical analysis, feature engineering, and visualization.

## Project Workflow

The notebook demonstrates:

* Synthetic employee data generation using Faker
* Object-oriented programming (OOP) for organizing the workflow
* PostgreSQL database storage and retrieval
* Database connectivity using psycopg2
* Data cleaning and transformation with Pandas
* Descriptive statistical analysis
* Feature engineering
* Salary standardization
* Dataset merging
* Data visualization with Matplotlib and Seaborn
* Grouped analysis and heatmap visualization

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

## Requirements

Before running the project, make sure you have:

* Python 3 installed
* Git installed
* Visual Studio Code
* Jupyter support in VS Code
* Access to a PostgreSQL database

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

Alternatively, open VS Code, select **File → Open Folder**, and select the `data-engineering-eda` folder.

### 3. Create a Virtual Environment

In the VS Code terminal, run:

```powershell
python -m venv .venv
```

This creates an isolated Python environment for the project.

### 4. Activate the Virtual Environment

On Windows PowerShell:

```powershell
.\.venv\Scripts\Activate.ps1
```

After activation, the terminal should display `(.venv)` at the beginning of the command prompt.

### 5. Install the Required Python Packages

Run:

```powershell
python -m pip install -r requirements.txt
```

This installs the Python libraries required by the project.

### 6. Configure the Database Connection

Create a file named:

```text
.env
```

in the root of the project.

Store the PostgreSQL connection information required by the notebook in this file.

The `.env` file should **not** be committed to GitHub because it may contain private database credentials.

### 7. Open the Jupyter Notebook

Open:

```text
data_engineering_eda.ipynb
```

in VS Code.

When prompted to select a Jupyter kernel, select the Python interpreter from the project's `.venv` environment.

You can verify that the notebook is using the correct environment with:

```python
import sys
print(sys.executable)
```

The path should point to:

```text
data-engineering-eda\.venv\Scripts\python.exe
```

### 8. Run the Notebook

In VS Code, select:

**Restart Kernel → Run All**

Run the notebook from top to bottom so that data generation, database operations, analysis, and visualizations execute in the intended order.

## Dataset

The primary employee dataset used in this project is generated programmatically using the Python Faker library rather than downloaded as a static external dataset.

The generated data contains employee information used throughout the database and exploratory data analysis workflow.

**Additional dataset:** Add the source link for the department dataset used during the dataset-merging portion of the notebook here.

## Technologies

* Python
* Jupyter Notebook
* PostgreSQL
* Pandas
* NumPy
* Faker
* psycopg2
* scikit-learn
* Matplotlib
* Seaborn

## Security

.env file not posted, will be emailed in a zip folder under subject line "9115726 - Data Engineering & EDA Workshop"
