#  SQL Server Data Warehouse

## Overview

To support scalable reporting and reliable analytics, a centralized SQL Server data warehouse was designed to integrate healthcare data from multiple sources into a single analytical model.

Rather than connecting Power BI directly to raw CSV files, the data was transformed into a structured dimensional model optimized for performance, consistency and maintainability.

The warehouse serves as the foundation of the Enterprise Healthcare Analytics Platform by providing clean, standardized and reusable data for reporting and decision-making.
## Why SQL Server?

SQL Server was selected because it provides a reliable relational database platform for managing structured healthcare data and supports enterprise reporting through:

- Efficient storage of large datasets
- High-performance querying
- Strong relational modelling
- Data integrity enforcement
- Reusable analytics views
- Seamless integration with Power BI

- ## Data Warehouse Architecture

The warehouse follows a dimensional modelling approach using a Star Schema.

This design separates descriptive business information into Dimension tables while transactional healthcare events are stored within Fact tables.

This architecture improves reporting performance, simplifies analytical queries and supports scalable dashboard development.

## Star Schema Design

### Dimension Tables

- DimPatient
- DimDate
- DimProvider
- DimOrganization
- DimPayer
- DimCondition
- DimProcedure
- DimMedication

### Fact Tables

- FactEncounter
- FactMedication
- FactProcedure
- FactCondition

- ## Why a Star Schema?

A dimensional model was chosen because it offers several advantages for Business Intelligence solutions.

These include:

- Faster dashboard performance
- Simpler analytical queries
- Reduced data redundancy
- Improved scalability
- Easier maintenance
- Better compatibility with Power BI

- ## Analytics Layer

To simplify reporting and reduce model complexity inside Power BI, dedicated SQL analytics views were created.

These views consolidate business logic and expose reporting-ready datasets for dashboard development.

Analytics views include:

- Patient Analytics
- Encounter Analytics
- Medication Analytics
- Procedure Analytics
- Condition Analytics

- ## SQL Responsibilities

The SQL layer was responsible for:

- Database creation
- Data import
- Data validation
- Data cleansing
- Warehouse modelling
- Fact table population
- Dimension table population
- Relationship management
- Analytics view creation

- ## Data Validation

Several validation checks were performed before reporting to ensure data reliability.

Examples include:

- Record count verification
- Date range validation
- Duplicate detection
- Null value assessment
- Foreign key validation
- Relationship consistency

- ## SQL Deliverables

This repository includes:

- Database creation scripts
- Dimension table scripts
- Fact table scripts
- Analytics view scripts
- Validation queries

- ## Business Value

The SQL Server data warehouse transforms raw healthcare data into a structured analytical repository that supports consistent reporting across executive, clinical, financial, medication and patient analytics dashboards.

By centralizing business logic within SQL, the reporting layer remains simpler, easier to maintain and more scalable for future enhancements.

## Design Decisions

Several architectural decisions were made during development to improve scalability and reporting performance.

These include:

- Using surrogate keys within dimension tables.
- Separating transactional and descriptive data.
- Creating reporting-ready SQL views.
- Standardizing business-friendly field names.
- Implementing a reusable dimensional model for future dashboard expansion.

- ## Outcome

The SQL Server data warehouse provides a reliable analytical foundation for the Enterprise Healthcare Analytics Platform, enabling fast, scalable and consistent reporting while reducing complexity within the Power BI semantic model.
