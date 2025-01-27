# Spare Parts Programming and Planning - A Data Analysis Automation Project

This repository showcases a **Material Planning System** developed in Python.

## Project Overview

This project aims to automate the data processing and analysis workflow for spare parts planning and inventory management. The current manual process involves working with over 50 Excel files, which are integrated and transformed into a consolidated DataFrame. This output allows detailed analysis of available inventory, sales history, ABC classification, inventory coverage, and purchase planning suggestions.

The project performs essential tasks in supply chain management, including stock control and logistics planning, supporting more strategic decision-making processes.

## Key Features

- **Data Normalization**: Standardizes material numbers across datasets for consistent analysis.
- **Automates manual workflows** for handling large datasets related to materials, inventory, sales, and parts per machine.
- **Consolidates multiple data sources** into a single, unified DataFrame.
- **Inventory Analysis**: Calculates stock levels, coverage, and costs.
- **Sales Analysis**: Processes historical sales data over 1, 12, 24, and 36 months.
- **ABC Classification**: Classifies materials based on their financial contribution and stock turnover.
- **Vendor and Planning Insights**: Analyzes supplier and lead time data for improved decision-making.
- **ETL pipeline** that extracts data from Excel files, transforms it (cleaning, normalizing, aggregating), and loads it into consolidated output files.

## Data Sources

The code extracts data from the following Excel files:

- **cod_df**: Contains material codes.
- **lx_df**: Inventory control data.
- **sp_df**: Stock cost information.
- **doc_df**: Sales history and ABC classification based on net value.
- **vor_df**: Historical planning data.
- **sales_block_df**: Items blocked from sales.
- **dispopara_df**: Planning restrictions, lead times, suppliers...
- **pintados_df**: Verification of raw materials.
- **class_df**: Item classification.
- **abc_rede_df**: Dealers' ABC classification.
- **mrp_df**: Responsible buyer.
- **va05_df**: Dealers' open sales orders data.
- **Other datasets**: Part numbers used for each machine model

## Data Processing Steps

1. **Data Extraction**: Reads data from various Excel files into pandas DataFrames.
2. **Data Transformation**:
   - **Normalization**: Cleans and standardizes columns (e.g., trimming whitespace, filling missing values, normalizing material codes).
   - **Data Cleaning**: Removes irrelevant columns and rows, filters out unwanted data.
   - **Aggregation and Calculation**: Computes stock value, ABC classification, and other key metrics.
   - **Merging**: Combines multiple datasets into a single DataFrame for consolidated analysis.
3. **Data Loading**: Exports the consolidated data back into Excel files for further reporting and analysis.

## Tech Stack

- **Python**: Core programming language.
- **Pandas**: Data manipulation and analysis.
- **NumPy**: Numerical calculations.
- **OpenPyXL**: Excel file formatting and styling.
- **Datetime**: Date operations for lead time and forecasting

## Installation

Installation

1. **Clone the repository**:

   git clone https://github.com/sabrinacosta1/spare-parts-programming-and-planning.git
   cd spare-parts-programming-and-planning

## Usage

To run the automation process, simply execute the Jupyter notebook or Python script:
1. Open the Jupyter notebook in your local environment:
2. Ensure that the necessary Excel files are available in the specified file paths.
3. Run all cells to perform the ETL process and generate the consolidated data output.

## Key Highlights
Real-World Impact: Solves critical challenges in inventory and production management.
Scalable Design: Supports additional datasets and machine types with minimal code changes.
Automation: Reduces manual effort by integrating data from multiple sources.
