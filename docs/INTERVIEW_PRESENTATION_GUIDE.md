# Interview presentation guide

## Ninety-second portfolio walkthrough

1. **Professional core:** “I work as a Data Analyst in media analytics, where I also own analytics-engineering responsibilities around recurring transformations, KPI consistency, validation and reporting delivery.”
2. **Public analytics proof:** “The TaskFlow case demonstrates how I diagnose product decline and connect metrics to business decisions.”
3. **Engineering transition:** “The SQL Server repository demonstrates three reproducible database projects, including greenfield development and maintenance.”
4. **Delivery layer:** “I added Terraform for a private Azure SQL target. It is validated; I distinguish that from a completed cloud deployment.”
5. **Boundary:** “Professional data/code remains confidential, so I publish synthetic analogues rather than employer assets.”

## Practical-task strategy

- Restate grain, keys, invariants and expected output before coding.
- Start with the simplest correct set-based solution.
- Add validation for nulls, duplicates, ranges and reconciliation.
- Explain retry/idempotency and failure handling.
- Inspect the execution plan before proposing an index.
- State what was executed versus what is only designed.
- Finish with assumptions, trade-offs and the next production-hardening step.

## Evidence language

Use:

- “implemented and validated locally”;
- “integration workflow is green on GitHub”;
- “independent lab using synthetic data”;
- “analytics-engineering responsibilities within my analyst role.”

Avoid:

- “production Azure deployment” before evidence exists;
- “commercial SQL Server/Databricks experience” if it was not used at work;
- unapproved internal metrics or screenshots.
