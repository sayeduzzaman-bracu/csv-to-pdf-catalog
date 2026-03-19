# Auto Catalog Pipeline

A Python-based automation pipeline that converts raw business data into clean, structured outputs and generates PDF catalogs automatically.

---

## Overview

This project demonstrates a complete data processing workflow:

Raw Data → Cleaning → Transformation → PDF Catalog + Summary Output

It is designed to handle real-world datasets, including messy transaction records, and convert them into professional, readable outputs with minimal manual work.

---

## Features

- Supports CSV input (structured business data)
- Data cleaning and normalization
- Transaction-to-product aggregation
- Automatic PDF catalog/report generation
- Pagination support for large datasets
- Summary CSV export
- Handles repeated entries and messy real-world data

---

## Use Case

This pipeline is useful for:

- Generating product catalogs from transaction data
- Converting CSV business data into reports
- Automating manual reporting workflows
- Preparing clean outputs for clients or internal use

---

## Project Structure

auto-catalog-pipeline/

│

├── input/                      # Input CSV files  
├── output/                     # Generated outputs  
│   ├── *_catalog.pdf  
│   └── *_product_summary.csv  
│  
├── main.py                     # Main pipeline script  
├── requirements.txt  
└── README.md  

---

## How It Works

1. Reads raw transaction data from CSV  
2. Cleans and standardizes fields  
3. Groups data into product-level summaries  
4. Generates:
   - PDF catalog/report
   - Summary CSV  

---

## Demo

Small Dataset:
- Clean structured data
- Demonstrates basic functionality

Real Dataset:
- Transaction-based data (1000+ rows)
- Demonstrates:
  - grouping logic
  - scalability
  - pagination handling

---

## Installation

pip install -r requirements.txt

---

## Usage

1. Place your CSV file inside the input/ folder  
2. Run:

python main.py

3. Check the output/ folder for results

---

## Output

- PDF Catalog / Report
- Cleaned & Aggregated CSV

---

## Notes

- Input data should contain fields like:
  Item, Category, Price, Quantity, etc.
- The system automatically groups repeated transaction entries into unique products

---

## Future Improvements

- Image support for product catalogs  
- Custom templates / branding  
- Multi-format input (Excel, JSON)  
- Web interface for uploads  

---

## Author

Built as part of a data automation portfolio focused on solving real-world business workflow problems.
