SME Analytics Benchmarks

This repository contains reproducible benchmarking scripts designed to evaluate the performance of multiple Python data analytics engines, including Pandas, Polars, and DuckDB, in the context of SME (Small and Medium Enterprise) data processing tasks. These experiments form part of a research project investigating trade-offs in scalability, efficiency, and prototyping speed among various modern data frameworks.

Purpose

The benchmarks aim to:
	•	Assess I/O loading speed for typical CSV SME datasets.
	•	Compare aggregation query performance across frameworks.
	•	Evaluate memory consumption patterns.
	•	Provide a transparent and replicable environment for future tests.

Repository Structure

benchmarks/
  benchmark_pandas.py
  benchmark_polars.py
  benchmark_duckdb.py
data/
  train.csv

	•	benchmark_pandas.py: Loads and analyzes with Pandas.
	•	benchmark_polars.py: Loads and analyzes with Polars.
	•	benchmark_duckdb.py: Runs SQL-like queries with DuckDB.
	•	data/train.csv: Sample dataset for reproducibility.

How to Run

First, activate your virtual environment:

source ../sme_env/bin/activate

Then install dependencies:

pip install pandas polars duckdb

Finally, run the scripts:

python benchmark_pandas.py
python benchmark_polars.py
python benchmark_duckdb.py

Research Context

These benchmarks support a broader MSc research project exploring advanced data pipeline architectures for SME analytics dashboards. The results will contribute to academic literature on data engineering trade-offs in modern Python ecosystems.

License

This repository is open-sourced under the MIT License.
