BMW Global Sales Data Analysis Using Apache PySpark

This project builds a scalable big-data pipeline using Apache PySpark to process, clean and analyze BMW worldwide sales data spanning 15 years from 2010 to 2024. 

The goal is to simulate a real data engineering workflow that a global automotive team would use to uncover regional trends, fuel type shifts, pricing patterns and model-level performance.

Pipeline Overview : 

The pipeline is structured across three phases. The first phase covers data extraction using PySpark CSV reader with automatic schema inference across 50,000 records and 11 features. 

The second phase covers data processing including schema standardization, missing value handling, categorical normalization, cross-field validation, IQR-based outlier detection and Z-score price anomaly detection. The third phase covers data visualization including top models by global sales, year-over-year sales trends from 2010 to 2024 and price distribution by fuel type across Diesel, Electric, Hybrid and Petrol.

Key Features :

Full PySpark pipeline with no pandas dependency, designed for scalability and reproducibility. Feature engineering including year-over-year growth, rolling 3-year averages, demand index, price deciles and mileage bands. Cohort analysis tracking how model age affects sales performance. Special handling for Electric and Hybrid vehicles with custom engine validation logic. Audit trail preserving original column values and boolean flags for every cleaned or removed record.

Tech Stack : Python, Apache PySpark, PySpark SQL, Matplotlib, Kaggle Dataset

Dataset : https://www.kaggle.com/datasets/ahmadrazakashif/bmw-worldwide-sales-records20102024
