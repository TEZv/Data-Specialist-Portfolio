# 🧭 Data engineering platform coverage

This is a capability-led evidence register, not a claim to qualify for every data engineering role. Middle is the target role; public implementation evidence and personal interview readiness are assessed separately.

## ✅ Verified platform run

[DE platform integration — successful run 34409326771](https://github.com/TEZv/lakehouse-finance-data-engineering/actions/runs/34409326771), implementation commit `b6db693`. All four jobs passed: **dbt**, **airflow**, **hive-hadoop**, **kubernetes**. The implementation was executed in disposable GitHub runners, not deployed into employer infrastructure or a paid cloud account. See [module instructions](https://github.com/TEZv/lakehouse-finance-data-engineering/tree/main/labs).

## Evidence register

| Capability | Technology | Actual evidence / next gate |
|---|---|---|
| Relational development | SQL Server / T-SQL | [Independent SQL labs](https://github.com/TEZv/mssql-data-engineering-portfolio); not commercial references |
| Batch lakehouse | Python, PySpark, Delta Lake | [Small synthetic pipeline](https://github.com/TEZv/lakehouse-finance-data-engineering); not a measured distributed production workload |
| Event transport and replay | Kafka, Python | [Kafka lab](https://github.com/TEZv/lakehouse-finance-data-engineering/tree/main/labs/kafka): producer, consumer, transactional SQLite sink, version handling, quarantine and replay; inspect the linked Actions result for broker execution status |
| Orchestration | Airflow | Implemented and CI-executed: batch → dbt DAG, actual retry after injected failure, two isolated logical dates via dag.test(); no scheduler/HA/backfill-service claim |
| Analytics transformation | dbt + DuckDB | Implemented and CI-executed: staging, per-key incremental fact, summary, uniqueness/null/relationship and reconciliation tests; initial/replay/correction/stale builds and generated docs |
| Cloud warehouse and security | Azure SQL, Storage, Data Factory, Key Vault | [ERP/DWH implementation](https://github.com/TEZv/mssql-data-engineering-portfolio/tree/main/projects/04-azure-erp-dwh-migration): star schema, source manifests, replay/version tests, ADF linked services/datasets/pipeline, managed identity, scoped RBAC, private endpoint definitions and failed-run alert. Terraform validated; Azure apply, endpoint approval, SQL data-plane grants and alert delivery remain live-run gates |
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

Employment confirmations are private documents. Independent lab technologies are not attributed to employment without factual support. Public technical references link code, tests and execution evidence only.

Interview practice stays in the learning track. Multiple-choice SQL drills establish individual concepts, not a professional grade.
