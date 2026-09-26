# Pipeline Health & Data Quality Dashboard

An end-to-end data quality monitoring pipeline built using Databricks and Snowflake.

## Project Overview

This project implements a data pipeline that ingests raw transactional data, performs data cleaning and transformation, applies data quality checks, generates Gold-level monitoring results, and exports the results to Snowflake for analytical querying.

## Architecture

```text
Raw CSV Data
     ↓
Databricks Bronze
     ↓
Databricks Silver
     ↓
Data Quality Checks
     ↓
Databricks Gold
     ↓
CSV Export
     ↓
Snowflake Stage
     ↓
Snowflake Tables
     ↓
Analytical SQL Queries
