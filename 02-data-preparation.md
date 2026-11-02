# 02 — Data preparation with Power Query

## Purpose

This note records how source data is brought into Power BI and prepared before it is loaded into the model.

## Source datasets described in the course

The transcript identifies these source queries/files:

- United States Sales
- Other Country Sales
- Customer
- Sales Territory
- Product
- Product Roll-up

The transcript refers to separate source files, including dimension data. The source files themselves are not included in this repository, so source paths and exact schemas must be recorded from the working environment.

## Power Query Editor orientation

The editor has three areas that are particularly useful when reviewing a query:

- **Queries pane:** lists the queries created in the Power Query project.
- **Data preview:** displays the data as it exists at the currently selected applied step.
- **Query Settings / Applied Steps:** records the sequence of transformations applied to the selected query.

The Applied Steps list is important documentation. It shows how the raw source was changed into a report-ready table and allows Power Query to repeat the sequence during refresh.

## Preparation workflow

### 1. Connect to the source

Connect to the relevant files or data sources. Confirm that the source path is valid and that the expected tables or files are available.

### 2. Inspect the data

Review:
- Column names and meanings
- Data types
- Row counts and column counts
- Null or blank values
- Duplicate records where relevant
- Unexpected values and inconsistent formats
- Whether the fields needed for the business questions are present

Do not remove or replace values without understanding their meaning.

### 3. Transform and cleanse

The course describes common preparation activities such as removing unneeded rows and columns, correcting unsuitable values, adding columns, and combining datasets.

Use only transformations that are appropriate for the actual source data. Record why each material transformation is required.

### 4. Merge queries

A merge joins columns from another query using one or more matching fields. It is useful when a table needs descriptive attributes stored in a separate table.

For every merge, document:
- Left/source query
- Right/lookup query
- Matching columns
- Join kind
- Whether the match is expected to be one-to-one, one-to-many, or otherwise
- How unmatched rows were reviewed

### 5. Append queries

An append stacks rows from tables with compatible structures. The course uses the United States Sales and Other Country Sales datasets as the example for combining sales records into a consolidated sales query.

Before appending, check that corresponding columns have compatible meanings and data types. A column with the same name is not necessarily semantically equivalent.

### 6. Create columns

Power Query can add columns derived from existing fields. Record the business purpose, source fields, output type, and transformation logic for each added column.

### 7. Load and review

Apply the transformations and load the prepared queries into the model. Confirm that:
- Expected queries are loaded
- Row counts are plausible
- Column types are correct
- No unexpected errors were introduced
- The model contains the fields required for relationships and reporting

## Refresh behaviour

Power Query stores transformation instructions. On refresh, Power BI re-runs those steps against the connected source. A refresh therefore depends on the source still being available and retaining a compatible structure.

## Query documentation template

Use this for each query:

```text
Query name:
Source file / connector:
Business purpose:
Important columns:
Applied Steps (in order):
1.
2.
3.
Merge details:
Append details:
Rows before / after:
Data-quality checks:
Known limitations:
Last reviewed:
```

## Important checks

- Use clear and consistent query and column names.
- Keep only the rows and columns needed for the analysis, where appropriate.
- Avoid changing source values without a documented reason.
- Recheck query steps when a source file or schema changes.
- Keep source paths and refresh requirements documented.
