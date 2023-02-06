# dbt-trino-date
## Installation
In your `packages.yml`:
```
packages:
  - git: "https://github.com/robbertDM/dbt-trino-date"
    revision: 0.1.0
```

In your `dbt_project.yml`:
```
dispatch:
  - macro_namespace: dbt_date
    search_order: ['dbt_trino_date', 'dbt_date']
```

Then, run `dbt deps`. You should be good to go.
