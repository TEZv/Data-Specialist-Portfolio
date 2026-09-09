# 🧭 Data engineering platform coverage

This is a capability-led evidence register, not a claim to qualify for every data engineering role. Middle is the target role; public implementation evidence and personal interview readiness are assessed separately.

## ✅ Verified platform run

[DE platform integration — successful run 34409326771](https://github.com/TEZv/lakehouse-finance-data-engineering/actions/runs/34409326771), implementation commit `b6db693`. All four jobs passed: **dbt**, **airflow**, **hive-hadoop**, **kubernetes**. The implementation was executed in disposable GitHub runners, not deployed into employer infrastructure or a paid cloud account. See [module instructions](https://github.com/TEZv/lakehouse-finance-data-engineering/tree/main/labs) and [Ukrainian interview walkthrough](https://github.com/TEZv/lakehouse-finance-data-engineering/blob/main/docs/PLATFORM_INTERVIEW_UA.md).

## Evidence register

| Capability | Technology | Actual evidence / next gate |
|---|---|---|
| Relational development | SQL Server / T-SQL | [Independent SQL labs](https://github.com/TEZv/mssql-data-engineering-portfolio); not commercial references |
| Batch lakehouse | Python, PySpark, Delta Lake | [Small synthetic pipeline](https://github.com/TEZv/lakehouse-finance-data-engineering); not a measured distributed production workload |
| Event transport and replay | Kafka, Python | [Kafka lab](https://github.com/TEZv/lakehouse-finance-data-engineering/tree/main/labs/kafka): producer, consumer, transactional SQLite sink, version handling, quarantine and replay; inspect the linked Actions result for broker execution status |
| Orchestration | Airflow | Implemented and CI-executed: batch → dbt DAG, actual retry after injected failure, two isolated logical dates via dag.test(); no scheduler/HA/backfill-service claim |
| Analytics transformation | dbt + DuckDB | Implemented and CI-executed: staging, per-key incremental fact, summary, uniqueness/null/relationship and reconciliation tests; initial/replay/correction/stale builds and generated docs |
| Cloud warehouse and security | One cloud first; Azure target already designed | Azure SQL Terraform exists; real deployment, least-privilege access, secret handling, measured cost and teardown evidence remain separate gates |
| Lakehouse service | Databricks | Job-definition draft only; adapt to an actual personal workspace and record a real run before claiming deployment |
| Hive/Hadoop ecosystem | Hive, HDFS/Hadoop | Implemented and CI-executed: real NameNode/DataNode, HiveServer2, external partitioned text table, row verification, external-file retention after table drop; single container, no HA/YARN/Kerberos |
| Container orchestration | Docker, Kubernetes | Implemented and CI-executed on kind: non-root restricted Job, ConfigMap, resource limits, expected failure and successful execution; temporary in-Pod storage, not a production cluster |
| Operations | Logging, freshness, reconciliation, access controls | Some tests/runbooks exist; no comprehensive observability, incident-response or governance implementation claimed |
| JVM development | Java / Kotlin | Optional job-specific track; no hands-on proficiency claimed merely from using Spark or Kafka |

## Completed scope and remaining gates

Completed: Kafka replay lab; shared replay-safe batch adapter; Airflow orchestration with failure recovery; dbt models/tests/docs; Hive/HDFS query lab; Kubernetes Job execution and diagnostics. These are modules of an independent lab portfolio, not six commercial projects.

Remaining: original PySpark pipeline correctness hardening (NULL routing, version conflicts, replay behavior and safe output handling); a controlled personal cloud deployment after account, budget and permissions are agreed; scale/HA/security hardening beyond the explicit lab boundaries; personal walkthrough and independent modification exercises.

Every module needs code, a reproducible run, assertions, limitations, an operational explanation, and an interview exercise. A checked-in configuration is not a successful deployment. No need to build AWS, Azure and GCP implementations simultaneously or add every warehouse product to the same system.

## Portfolio and professional references

Public technical references mean links to code, tests, CI runs and design explanations. Employer references mean a consenting manager/HR contact confirming work actually performed. These are different forms of evidence.

The [manager confirmation template](REFERENCE_CONFIRMATION_TEMPLATE.md) must not attribute Kafka, Spark, Kubernetes or any other independent lab technology to employment unless it was actually used there. Dates, job titles and scope remain factual.

Interview practice stays in the learning track. Multiple-choice SQL drills establish individual concepts, not a professional grade.
