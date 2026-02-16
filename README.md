# 📘 MSDS 459 - Knowledge Engineering
**Course:** MSDS 459 - Knowledge Engineering  
**Term:** Winter 2026  
**Student:** Syed Mehdi  

### MSDS 459 — Week 06 Checkpoint B

This repository contains my submission for Checkpoint B: Data and Schema for the Knowledge Graph.

The objective of this checkpoint is to define and implement the data sources, schema design, and database architecture for the term project knowledge base. The project adopts a hybrid database architecture, combining PostgreSQL (structured + JSONB storage) with Memgraph (graph analytics layer).

## Structure

```
.
├── companies.csv
├── data/
│   ├── financial/
│   │   └── yahoo/
│   │       ├── ABBV.csv
│   │       ├── AMGN.csv
│   │       ├── ...
│   │       └── PFE.csv
│   ├── news/
│   │   └── gdelt_articles.jsonl
│   └── regulatory/
│       └── fda_docs.jsonl
├── memgraph/
│   ├── schema_healthcare.cypher
│   └── schema_postgres_healthcare.sql
├── Crawler-CheckPoint-B.ipynb
└── README.md
```


## Data Sources

This project integrates multiple structured and unstructured data sources:

1. Financial Market Data (Yahoo Finance)
2. Regulatory Documents (FDA)
3. News Data (GDELT API)

