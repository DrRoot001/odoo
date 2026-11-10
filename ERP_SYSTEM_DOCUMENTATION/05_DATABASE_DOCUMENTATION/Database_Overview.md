# Database Overview

## Engine and access

The declared database engine is PostgreSQL; packaging requires `psycopg2`, and release metadata states PostgreSQL 16 minimum (`odoo/release.py:32`). Odoo models are declared in Python and materialized into PostgreSQL through the registry/module loading process. This repository does not contain one static SQL schema representing all possible installed addons.

## Model inventory

Static model metadata was found in 4,204 class definitions. The full machine-readable dictionary is `Entity_Dictionary.csv`. It records source file, class, `_name`, `_inherit`, and `_inherits` values where literal metadata was available.

## Important limitation

Table names, columns, indexes, constraints, and relationship cardinalities can vary with installed addons, inherited models, PostgreSQL version, configuration, and migrations. A definitive deployed schema requires a live database dump or registry introspection.
