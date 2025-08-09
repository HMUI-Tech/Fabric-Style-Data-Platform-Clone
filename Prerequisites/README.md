# 0) Python packages
- psycopg2-binary
  The Postgres driver for Python. It’s how your Python code talks to your PostgreSQL database (run SQL, load data, etc.).
- pandas
  For working with tabular data (CSV, Excel, JSON). it'll be used to read files, clean columns, and hand clean data off to the database.
- pyarrow
  A fast columnar memory format (Arrow) + tools for Parquet. Arrow makes some pandas operations faster and more efficient.
- dbt-progres
  dbt (data build tool) but for Postgres. dbt handles dependencies, builds tables/views in the right order, and runs data tests.
  It is the “transform” engine (Fabric-like).
- pydantic
  Helpful for validating and parsing configuration or file schemas in Python. If your pipeline expects certain columns/types, Pydantic can enforce that before loading.
- python-dotenv
  Lets you keep secrets (DB URL, passwords) in a .env file and load them into your script via environment variables. Cleaner and safer than hard-coding
