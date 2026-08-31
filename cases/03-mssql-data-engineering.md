# Case 3 — MS SQL Server Data Platform

**Classification:** Data Engineering / Database Development

**Context:** independent portfolio lab, synthetic data

**Evidence:** public code, automated assertions, CI and Terraform

## Scope

- Greenfield retail ERP order-to-cash database and reporting layer.
- Media performance mart maintenance and late-arriving corrections.
- SQL Server reliability toolkit for integrity, indexes, statistics, retention, backups and Query Store diagnostics.
- Private-network Azure SQL deployment target defined with Terraform.

## Engineering evidence

- T-SQL stored procedures, views and an inline table-valued function.
- SCD Type 2 history, transactions, idempotency and error handling.
- Constraints, reconciliation, audit/reject paths and executable assertions.
- Docker/GitHub Actions SQL Server integration workflow.
- Portable Terraform, locked providers and Azure SQL infrastructure validation.

## Current verification boundary

Terraform is implemented and locally validated. SQL Server runtime status is shown by the GitHub Actions workflow. A real Azure deployment is not claimed until a controlled `plan/apply/smoke-test/destroy` evidence pack exists.

Inspect the complete repository: [mssql-data-engineering-portfolio](https://github.com/TEZv/mssql-data-engineering-portfolio).
