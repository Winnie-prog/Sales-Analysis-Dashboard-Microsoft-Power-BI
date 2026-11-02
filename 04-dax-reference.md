# 04 — DAX reference

## Purpose

This file is a durable reference for DAX expressions used in the report. Add the exact formulas from the PBIX rather than relying on remembered or generic versions.

## DAX concepts covered

### Expressions

DAX is the expression language used in Power BI for calculations in the data model.

### Calculated columns

A calculated column produces a value for each row in a table. It is evaluated as part of model processing/refresh and stored in the model.

### Measures

A measure is evaluated when it is used in a visual or query. Its result responds to the current filter context, including slicers, filters, and selections.

### Filter context

Filter context is the set of filters that apply when a calculation is evaluated. For example, selecting a year or continent changes the context in which a sales measure is calculated.

### Time intelligence

Time-intelligence calculations support comparisons and analysis across dates and periods. They depend on a suitable date table and correct date relationships.

### Quick Measures

Power BI Quick Measures provide a guided way to create certain common calculations. Review the generated expression so that its logic is understood before relying on it.

## Measures visible in the report

The report overview indicates metrics including Total Sales, a Sales Target, and Profit Margin by product category. The exact DAX definitions must be copied from the PBIX model and recorded below.

### Measure register

| Measure name | Business definition | Format | Used in | Verified? |
|---|---|---|---|---|
| Total Sales | Total sales value according to the model's sales definition | Confirm in model | KPI / report | No |
| Sales Target | Target value used for comparison | Confirm in model | KPI / report | No |
| Profit Margin | Margin calculation used for product-category comparison | Confirm in model | Category visual | No |

## Reusable documentation template

Copy this block for every measure:

```text
## Measure: [Exact measure name]

### Business purpose
What question does this measure answer?

### DAX formula
Paste the exact formula from Power BI Desktop.

### Explanation
Explain each function and important part of the expression.

### Evaluation context
Which filters, relationships, or slicers affect the result?

### Format
Currency / percentage / whole number / decimal / other.

### Used in
Report page and visual name.

### Validation
How was the result checked against source data or another trusted calculation?

### Notes
Assumptions, limitations, dependencies, and future changes.
```

## Reusable calculated-column template

```text
## Calculated column: [Exact column name]

Table:
DAX expression:
Purpose:
Row-level meaning:
Data type:
Where used:
Validation:
Notes:
```

## DAX review checklist

- [ ] Exact formula copied from the model.
- [ ] Measure name communicates its meaning.
- [ ] Format string is appropriate.
- [ ] Filter-context behaviour is understood.
- [ ] Date calculations use the intended date relationship.
- [ ] Results have been validated against a known total or sample.
- [ ] Dependencies on other measures are documented.

> Do not publish placeholder formulas as if they were the formulas used in this report. Replace the register and templates with verified model expressions as you inspect the PBIX.
