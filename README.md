# etl-data-quality-testing
During my work at various companies, I noticed we were spending too much time manually checking data quality after ETL runs. I built this SQL-based framework to automate common data validation checks
etl-data-quality-testing/
├── README.md
├── sql_scripts/
│   ├── 01_setup_test_tables.sql
│   ├── 02_data_quality_checks.sql
│   ├── 03_comparison_tests.sql
│   └── 04_generate_test_report.sql
├── sample_data/
│   ├── source_customers.csv
│   ├── target_customers.csv
│   └── daily_orders.csv
├── test_results/
│   └── sample_test_report.html
└── documentation/
    ├── test_scenarios.md
    └── how_to_use.md


# ETL Data Quality Testing Framework

## Overview
A simple SQL-based framework I developed to automate data quality checks during ETL processes. 

## Problem Solved
- Manual data validation was time-consuming
- Inconsistent testing across different ETL jobs
- Data quality issues discovered too late in the process

## What It Does
- **Row Count Validation**: Ensures no data loss during ETL
- **Duplicate Detection**: Identifies duplicate records
- **Null Value Checks**: Validates required fields
- **Data Type Validation**: Ensures proper data formats
- **Business Rule Testing**: Custom validation rules

## Technologies
- SQL Server / PostgreSQL
- T-SQL / PL/pgSQL
- Simple HTML reporting

## Quick Start
1. Run `01_setup_test_tables.sql` to create test framework
2. Modify `02_data_quality_checks.sql` for your tables
3. Execute tests and review HTML report

## Real-World Impact
- Reduced manual testing time by 70%
- Caught data quality issues 2 days earlier
- Standardized testing across 5 different ETL processes
