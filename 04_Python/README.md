#  Python Data Profiling & Quality Assurance

## Overview

Reliable analytics begins with reliable data.

Before loading healthcare records into the SQL Server data warehouse, Python was used to profile, validate and assess the quality of the raw datasets. This ensured that inconsistencies, structural issues and potential data quality problems were identified early in the analytics pipeline.

Rather than using Python for machine learning, this project focuses on practical data engineering tasks that improve the accuracy, reliability and maintainability of Business Intelligence solutions.
## Why Python?

Python was selected because it provides a flexible and efficient way to automate data profiling and quality assurance tasks before the data enters the warehouse.

The Python layer was responsible for:

- Profiling healthcare datasets
- Validating dataset structures
- Assessing data quality
- Detecting inconsistencies
- Producing documentation that supports downstream analytics
- ## Python Workflow

The Python layer follows a structured workflow before data is loaded into SQL Server.

Raw CSV Files

↓

File Profiling

↓

Schema Validation

↓

Data Quality Assessment

↓

Relationship Validation

↓

Data Dictionary Generation

↓

SQL Server Data Warehouse
## Python Components

The project includes several reusable Python modules designed to automate common data quality tasks.

### File Profiler

Reviews each source dataset and summarizes:

- File size
- Number of rows
- Number of columns
- Data types
- Basic metadata

---

### Schema Profiler

Validates the structure of each dataset by checking:

- Column names
- Missing columns
- Unexpected columns
- Data types

---

### Quality Profiler

Evaluates the overall quality of the data by identifying:

- Missing values
- Duplicate records
- Invalid values
- Data completeness

---

### Relationship Profiler

Assesses relationships between datasets and verifies that key fields align correctly across the healthcare model.

---

### Report Generator

Produces structured profiling reports that summarize the overall health of the datasets and provide documentation for the analytics process.
## Why Data Profiling Matters

Healthcare reporting depends on accurate and trustworthy data.

Automated profiling reduces the likelihood of:

- Inconsistent reporting
- Missing records
- Invalid relationships
- Data quality issues
- Incorrect analytical conclusions

By validating the data before warehouse loading, the reporting layer becomes significantly more reliable.
## Automation

Python scripts were designed to be reusable so that new healthcare datasets can be assessed with minimal manual effort.

This approach supports:

- Faster onboarding of new datasets
- Consistent quality checks
- Repeatable validation processes
- Improved maintainability
- ## Business Value

The Python layer improves confidence in the analytical solution by ensuring that only validated and well-understood data progresses into the SQL Server data warehouse.

This reduces reporting errors and establishes a strong foundation for executive, clinical and financial decision-making.
## Python Libraries

The solution was developed using commonly adopted Python libraries including:

- pandas
- pathlib
- os
- numpy
- openpyxl
- sqlalchemy
- pyodbc
- ## Outcome

The Python layer provides an automated and repeatable approach to healthcare data profiling and validation, ensuring that the SQL Server data warehouse receives consistent, high-quality data for downstream analytics and reporting.
