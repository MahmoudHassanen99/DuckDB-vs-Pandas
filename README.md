# DuckDB vs Pandas: Performance Benchmark for CSV & Parquet Processing

## Overview
This project benchmarks **DuckDB** against **Pandas** for loading and aggregating **CSV and Parquet files**. It explores:
- **Load Time**: Comparing CSV vs Parquet with Pandas & DuckDB
- **Aggregation Performance**: Speed comparison for `groupby`
- **Multi-Core Efficiency**: DuckDB's threading advantage

## Key Observations
✅ **Parquet is much faster than CSV** for both Pandas & DuckDB  
✅ **DuckDB significantly outperforms Pandas** in loading and aggregation  
✅ **Multi-core processing with DuckDB** results in near-instant file loads  

**Example Results:**
| Method | Small CSV (s) | Small Parquet (s) | Large CSV (s) | Large Parquet (s) |
|--------|--------------|------------------|--------------|------------------|
| Pandas | 1.25 | 0.21 | 5.30 | 0.53 |
| DuckDB | 0.60 | 0.42 | 2.44 | 1.98 |
| DuckDB (4 cores) | x | x | 0.0619 | 0.001 |

## 📂 Repository Structure
- `notebooks/` → Jupyter notebooks for step-by-step analysis
- `data/` → Sample datasets (not included in repo)

