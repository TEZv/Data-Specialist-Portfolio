# 🧭 Data engineering platform coverage

This is a capability-led expansion plan, not a claim to qualify for every data engineering role. Middle is the target role; public implementation evidence and personal interview readiness are assessed separately.

## Evidence register

| Capability | Technology | Actual evidence / next gate |
|---|---|---|
| Relational development | SQL Server / T-SQL | [Independent SQL labs](https://github.com/TEZv/mssql-data-engineering-portfolio); not commercial references |
| Batch lakehouse | Python, PySpark, Delta Lake | [Small synthetic pipeline](https://github.com/TEZv/lakehouse-finance-data-engineering); not a measured distributed production workload |
| Event transport and replay | Kafka, Python | [Kafka lab](https://github.com/TEZv/lakehouse-finance-data-engineering/tree/main/labs/kafka): producer, consumer, transactional SQLite sink, version handling, quarantine and replay; inspect the linked Actions result for broker execution status |
| Orchestration | Airflow | Planned: schedule a bounded existing pipeline, dependency/retry policy, failed-task recovery and backfill tests |
| Analytics transformation | dbt | Planned: staging and marts, grain, incremental model, uniqueness/null/relationship tests, metric definitions and reconciliation |
| Cloud warehouse and security | One cloud first; Azure target already designed | Azure SQL Terraform exists; real deployment, least-privilege access, secret handling, measured cost and teardown evidence remain separate gates |
| Lakehouse service | Databricks | Job-definition draft only; adapt to an actual personal workspace and record a real run before claiming deployment |
| Hive/Hadoop ecosystem | Hive, HDFS/Hadoop | Planned separate compatibility lab: external tables, partitions, file formats and metastore vs storage. Not required to run Kafka; do not imply HDFS is part of every lakehouse |
| Container orchestration | Docker, Kubernetes | Container-based CI exists. Kubernetes lab planned: a batch Job, resources, configuration, probes where applicable and failed-run diagnostics; not a production cluster |
| Operations | Logging, freshness, reconciliation, access controls | Some tests/runbooks exist; no comprehensive observability, incident-response or governance implementation claimed |
| JVM development | Java / Kotlin | Optional job-specific track; no hands-on proficiency claimed merely from using Spark or Kafka |

## Delivery order and acceptance criteria

1. Kafka replay lab with unit tests and broker CI.
2. Existing lakehouse correctness hardening: NULL routing, version conflicts, replay behavior, safe output handling and accurate metric names.
3. Airflow orchestration of an existing batch; demonstrate a failure and safe rerun.
4. dbt analytics layer with a documented input contract and hand-checked metric.
5. Controlled personal cloud deployment after account, budget and permissions are agreed.
6. Hive/Hadoop and Kubernetes as bounded optional modules with their own execution evidence.

Every module needs code, a reproducible run, assertions, limitations, an operational explanation, and an interview exercise. A checked-in configuration is not a successful deployment. No need to build AWS, Azure and GCP implementations simultaneously or add every warehouse product to the same system.

## Portfolio and professional references

Public technical references mean links to code, tests, CI runs and design explanations. Employer references mean a consenting manager/HR contact confirming work actually performed. These are different forms of evidence.

The [manager confirmation template](REFERENCE_CONFIRMATION_TEMPLATE.md) must not attribute Kafka, Spark, Kubernetes or any other independent lab technology to employment unless it was actually used there. Dates, job titles and scope remain factual.

Interview practice stays in the learning track. Multiple-choice SQL drills establish individual concepts, not a professional grade.
