---
title: SQL Query Optimizer
industry: coding
tags: [sql, performance, database, optimization, query]
models: [claude, gpt-4, llama]
contributor: justfathi
---

## Description
Analyzes a slow or complex SQL query, identifies performance problems, and rewrites it with specific optimizations — including index recommendations, join improvements, and execution plan guidance.

## Use Case
Backend developers and data engineers who need to improve a slow query and understand why it's slow, without spending hours reading documentation or waiting for a DBA review.

## The Prompt
```
You are a database performance expert. Analyze the SQL query below and provide a structured optimization report.

**SQL QUERY OPTIMIZATION REPORT**

**1. What the query does**
[Plain English explanation of what this query retrieves — no SQL jargon]

**2. Performance problems identified**
[List each problem with an explanation of why it's expensive:]
- [Problem]: [Why it's slow / what the cost is]

**3. Optimized query**
```sql
-- Optimized version
[REWRITTEN QUERY HERE]
```

**4. What changed and why**
[For each change made, explain:]
- Change: [What was modified]
- Reason: [Why this is faster]
- Expected impact: [High / Medium / Low — with a brief explanation]

**5. Index recommendations**
[List specific indexes to create that would improve this query:]
```sql
-- Recommended indexes
CREATE INDEX idx_[table]_[column] ON [table]([column]);
```
[For each index, explain why it helps and what queries benefit from it]

**6. Execution plan guidance**
[What to look for in EXPLAIN / EXPLAIN ANALYZE to verify improvement — e.g., "confirm seq scan on orders is replaced by index scan"]

**7. Risks and caveats**
[Any trade-offs: indexes that slow down writes, locking behavior, query result differences to verify]

---

Query context:
Database: [PostgreSQL / MySQL / SQLite / SQL Server / BigQuery / Snowflake / other]
Table sizes (approximate): [e.g., "orders: 10M rows, users: 500K rows"]
Current query performance: [e.g., "runs in 8 seconds, times out on large datasets"]
Schema (paste relevant CREATE TABLE or describe key columns):
```sql
[PASTE SCHEMA HERE]
```

Query to optimize:
```sql
[PASTE QUERY HERE]
```

EXPLAIN output (if available):
```
[PASTE EXPLAIN OUTPUT HERE]
```
```

## Notes
- Table size matters enormously — a query that's fine at 10K rows can be catastrophic at 10M; always provide approximate row counts
- Paste the EXPLAIN / EXPLAIN ANALYZE output if you have it — it tells the model exactly what the database is doing
- Index recommendations are suggestions — test write-performance impact before adding indexes to write-heavy tables
- For data warehouse queries (BigQuery, Snowflake), optimization focuses on partition pruning and clustering rather than traditional indexes
