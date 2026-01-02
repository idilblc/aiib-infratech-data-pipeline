# aiib-infratech-data-pipeline
AIIB Infratech Portal 
# AIIB InfraTech Portal – Python Data Pipeline

This project demonstrates a Python-based data analytics pipeline built to collect,
clean, and export company-level data from the AIIB InfraTech public API.

## Problem
Public infrastructure and climate-tech datasets are often exposed via APIs with
pagination, nested JSON, and inconsistent text formatting, making them difficult
to use directly for analysis.

## Solution
I built a reproducible Python pipeline that:
- Ingests data from a production REST API
- Handles pagination and request throttling
- Normalises nested JSON into a tabular format
- Applies text sanitisation to ensure Excel compatibility
- Exports clean CSV and Excel outputs for downstream analysis

## Dataset
- ~1,100+ infrastructure and infra-tech companies
- Publicly available data from the AIIB InfraTech Portal
- No authentication or restricted data used

## Key Python Skills Demonstrated
- API interaction with `requests`
- Pagination and rate limiting
- JSON normalisation with `pandas`
- Data cleaning and validation
- Excel-safe export handling
- Notebook-based analytical documentation

## Notes on Data Limitations
The company list endpoint does not expose thematic tags.
Full classification would require enrichment via a detail-level API.

## How to Run
```bash
pip install -r requirements.txt
jupyter notebook
