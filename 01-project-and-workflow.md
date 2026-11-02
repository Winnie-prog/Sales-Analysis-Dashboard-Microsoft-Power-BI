# 01 — Project and workflow

## Purpose of this note

This file records the business context and the end-to-end sequence followed when developing the AdventureWorks Sales Analysis report.

## Business scenario

The course scenario places the analyst in AdventureWorks Cycles. The business wants a more useful way to review sales performance than its existing Excel process. The described limitations include a time-consuming preparation process, reporting only a couple of times per month, limited detail, limited interactivity, and difficulties distributing and controlling report versions.

The target analysis is expected to cover three years and allow users to analyze sales by product, sales territory, customer, and date at daily detail.

## Business questions

Use these questions to guide report design and future enhancements:

1. What are total sales, and how do they compare with the target?
2. How does sales performance change across time?
3. Which geographical areas contribute to sales?
4. How do product categories compare in terms of profit margin?
5. What detail should a user be able to access after identifying an unusual or interesting result?

## Analytics lifecycle

The workflow is iterative rather than strictly one-way:

1. Acquire data.
2. Understand the data and its business meaning.
3. Validate assumptions and investigate uncertainty.
4. Transform and prepare data for reporting.
5. Analyze the prepared data.
6. Present findings.
7. Use questions raised by the report to refine earlier steps.

A report should not be treated as reliable merely because it renders successfully. The analyst must understand the source, definitions, business rules, and limitations behind the figures.

## Development sequence

| Stage | Main activity | Output |
|---|---|---|
| Requirements | Translate the business request into analytical questions | Defined reporting scope |
| Acquisition | Connect to the relevant source files | Imported queries |
| Preparation | Clean, shape, merge, and append data | Report-ready queries |
| Modelling | Organize tables and relationships | Usable semantic model |
| Calculations | Create DAX expressions and measures | Reusable business calculations |
| Reporting | Design visuals and interactions | Interactive report |
| Distribution | Publish and manage access | Report available to intended users |

## Scope and verification

The supplied transcript covers the broader Power BI lifecycle. The PBIX file is the artifact to inspect when confirming which steps, measures, and report interactions are present in this particular implementation. Do not mark a feature as implemented until it has been checked in Power BI Desktop.

## Notes to add during future reviews

- Business definition of sales:
- Definition of sales target:
- Definition of profit margin:
- Reporting period:
- Intended report audience:
- Known data limitations:
- Outstanding business questions:
