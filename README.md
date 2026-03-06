# VectorQL
Columnar Analytics Engine or a mini DuckDB from scratch.

# Architecture
A rough sketch rn
```
SQL parser
   |
logical plan
   |
vectorized execution engine
   |
columnar storage
```

# Minimum features

### Storage

- columnar layout

- Parquet reader

### Execution

- vectorized operators

- aggregation

- filtering

- group by

### Optimization

- predicate pushdown

- column pruning

# Target metrics

### Dataset size

- 10M+ rows processed

### Performance

- 5–10× faster than row store scan

- queries under 200 ms for aggregations

### Memory

- vectorized batches (1024 rows)
