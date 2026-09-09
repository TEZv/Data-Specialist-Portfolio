# 🏞️ Lakehouse Data Engineering — PySpark & Delta Lake

## Positioning

**Area:** Data Engineering / Lakehouse Engineering  
**Evidence type:** independent, reproducible portfolio project  
**Commercial claim:** none

## Business scenario

A synthetic financial-events feed needs to remain auditable in raw form, be cleaned and corrected, and then serve daily trading-activity and cash-flow outputs. These are not a full position or risk-exposure calculation.

## What is implemented

- PySpark transformations with Delta Lake tables;
- Bronze / Silver / Gold lakehouse layers;
- schema evolution: a late source batch introduces `trade_venue`;
- explicit validation and quarantine for invalid trade events;
- Delta `MERGE` upsert for late corrections; current replay test covers Silver row count, not full-pipeline idempotency;
- Gold aggregates for daily account/instrument activity and cash flow;
- PySpark/Delta integration tests in GitHub Actions;
- Databricks Asset Bundle job definition for a future personal-workspace run.

## 🧩 Platform extension

The companion [platform modules](https://github.com/TEZv/lakehouse-finance-data-engineering/tree/main/labs) add Kafka transport/replay, a shared Python batch, Airflow → dbt orchestration, Hive queries over real HDFS and Kubernetes batch Jobs. All four new platform jobs passed in [run 34409326771](https://github.com/TEZv/lakehouse-finance-data-engineering/actions/runs/34409326771).

The extension uses a deliberately small integer event fixture. It is not a production finance system or a Kafka-to-Spark integration. See [coverage and limitations](../docs/PLATFORM_COVERAGE.md).

## Evidence and boundary

Inspect the code, tests and CI status in [lakehouse-finance-data-engineering](https://github.com/TEZv/lakehouse-finance-data-engineering).

This is an independent project built with synthetic data. It demonstrates implementation ability in PySpark/Delta patterns; it does not imply commercial Databricks delivery or production-scale operations.
