# 🏞️ Lakehouse Data Engineering — PySpark & Delta Lake

## Positioning

**Area:** Data Engineering / Lakehouse Engineering  
**Evidence type:** independent, reproducible portfolio project  
**Commercial claim:** none

## Business scenario

A synthetic financial-events feed needs to remain auditable in raw form, be cleaned and corrected incrementally, and then serve daily exposure and cash-flow outputs to BI or risk consumers.

## What is implemented

- PySpark transformations with Delta Lake tables;
- Bronze / Silver / Gold lakehouse layers;
- schema evolution: a late source batch introduces `trade_venue`;
- explicit validation and quarantine for invalid trade events;
- idempotent Delta `MERGE` upsert for late corrections;
- Gold aggregates for account/instrument exposure and cash flow;
- PySpark/Delta integration tests in GitHub Actions;
- Databricks Asset Bundle job definition for a future personal-workspace run.

## Evidence and boundary

Inspect the code, tests and CI status in [lakehouse-finance-data-engineering](https://github.com/TEZv/lakehouse-finance-data-engineering).

This is an independent project built with synthetic data. It demonstrates implementation ability in PySpark/Delta patterns; it does not imply commercial Databricks delivery or production-scale operations.
