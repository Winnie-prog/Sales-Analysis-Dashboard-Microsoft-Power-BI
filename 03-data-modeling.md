# 03 — Data modeling

## Purpose

This note explains the modelling concepts covered in the course and provides a place to record the actual structure of the Sales Analysis PBIX.

## Why the model matters

The data model determines how tables work together in calculations and report visuals. A report can look correct while still producing misleading results if relationships, keys, or filter behaviour are not understood.

## Dimensional modelling

The course introduces dimensional modelling and star-schema principles. In a typical analytical model:

- A **fact table** stores business events or measurable transactions.
- **Dimension tables** provide descriptive context used to group, filter, and analyze those events.

For this sales scenario, the subject areas include sales, customer, product, sales territory, and date. Confirm the exact table names and roles in the PBIX Model view before documenting them as the final model design.

## Relationships

Relationships connect tables through matching key columns.

When reviewing or creating a relationship, record:

- Table on each side
- Column on each side
- Cardinality
- Cross-filter direction
- Active or inactive status
- Whether the key is unique on the expected side
- Any unmatched or blank keys

Do not assume relationship settings. Confirm them in Model view.

## Date table and order date

The course includes building a date table and creating a relationship between the order date and sales. A dedicated date table supports consistent time-based analysis and provides calendar attributes for grouping and filtering.

When reviewing the implementation, check:
- Date table range
- Unique date values
- Continuous date coverage
- Date data type
- Relationship to the sales order-date field
- Whether the date table is marked as a date table, where appropriate
- Whether additional date relationships exist and whether they are active

## Column groups and hierarchies

The course also covers creating column groups and hierarchies. Hierarchies let users navigate from summarized categories to more detailed levels. The order and meaning of hierarchy levels should match the business structure.

## Model organization

Good model hygiene includes:
- Clear table, column, and measure names
- Removing unused fields from the reporting model where appropriate
- Appropriate data types and formats
- Sensible default summarization
- Useful descriptions and data categorization
- Organizing measures and related fields for easier maintenance

## Model inventory — complete from the PBIX

| Table | Role (fact/dimension) | Key column(s) | Related tables | Notes |
|---|---|---|---|---|
|  |  |  |  |  |
|  |  |  |  |  |
|  |  |  |  |  |

## Relationship register — complete from Model view

| From table/column | To table/column | Cardinality | Cross-filter | Active? | Reason / notes |
|---|---|---|---|---|---|
|  |  |  |  |  |  |

## Validation checklist

- [ ] Fact and dimension roles are understood.
- [ ] Relationship keys have been checked.
- [ ] Cardinality is appropriate for the data.
- [ ] Filter direction is intentional.
- [ ] Date table and order-date relationship are reviewed.
- [ ] Hierarchies reflect the business structure.
- [ ] Unused columns and ambiguous relationships have been reviewed.
