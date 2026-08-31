# Case 1 — Media Reporting Automation

**Classification:** Analytics Engineering / BI Engineering responsibilities within a Data Analyst role

**Context:** professional media analytics

**Disclosure:** anonymized; no proprietary source code, credentials, raw data, internal screenshots or confidential business values

## Business need

Stakeholders needed repeatable performance reporting across content, channels, projects and reporting periods. The work had to reconcile platform exports and metadata, preserve agreed KPI logic, reduce manual preparation, and deliver understandable dashboards/workbooks.

## My contribution

- Prepared and validated data used in recurring content-performance reporting.
- Automated parts of extraction, transformation and workbook/report generation with Python, SQL and spreadsheet tooling.
- Worked with YouTube/platform metadata, views, revenue and audience-retention measures.
- Implemented view-weighted retention logic instead of mathematically incorrect simple averages.
- Maintained project/subproject mapping and reporting filters.
- Added delivery checks for missing mappings, broken formulas, unexpected zeroes and inconsistent totals.
- Produced reporting outputs for business users in Power BI, Looker Studio, Excel and Google Sheets contexts.

## Why this is partly Analytics Engineering

The analytical interpretation is Data Analytics. The repeatable transformation logic, shared KPI definitions, quality controls, mapping layer and stable reporting outputs are Analytics Engineering / BI Engineering responsibilities.

## System pattern

```text
platform APIs / exports / metadata
              |
              v
       validated registry
              |
              v
 Python + SQL transformations
              |
       +------+------+
       |             |
       v             v
 quality checks   metric layer
       |             |
       +------+------+
              v
 dashboards / delivery workbooks
```

## Quality rules

- Retention is weighted by views.
- Scope is controlled through an explicit content registry/mapping.
- Primary publications are distinguished from duplicates/reposts where required.
- Revenue, views and retention totals are reconciled before delivery.
- Confidential data never enters public portfolio fixtures.

## Public evidence boundary

The original production implementation and data remain private. A synthetic analogue of the database patterns, weighted-retention logic, audits and assertions is available in the [MS SQL Server Data Engineering Portfolio](https://github.com/TEZv/mssql-data-engineering-portfolio/tree/main/projects/02-media-performance-mart).

This link demonstrates the engineering pattern; it is not presented as the employer's source code.

## Interview summary

> In my professional role I work with media-performance reporting and automation. The business-facing part is analytics; the repeatable transformation, KPI, mapping and validation layer is analytics engineering. Because the source data and code are confidential, I built a synthetic public implementation that demonstrates the same engineering principles without reproducing employer assets.
