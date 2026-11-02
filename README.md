# Sales Analysis Dashboard | Microsoft Power BI

> A working technical notebook documenting the development, structure, and reference notes for an AdventureWorks sales-analysis report.

## Project purpose

This repository records the end-to-end workflow used to develop a sales-analysis solution in Power BI. It is intended to serve two purposes:

1. **Project record:** explain the business scenario, analytical questions, tools, and report structure.
2. **Personal technical reference:** preserve the workflow, concepts, formulas, modelling decisions, and troubleshooting notes so they can be revisited and extended later.

The source learning material is the *Complete Guide to Power BI for the Data Analyst* transcript supplied with this project. The PBIX file is included as the working report.

## Business scenario

The AdventureWorks scenario starts with a request to make sales information easier to analyze. The existing Excel-based process is described as slow to prepare, infrequently distributed, limited in detail and interactivity, and difficult to distribute consistently.

The intended Power BI solution supports analysis by date, product, sales territory, and customer, with more timely and interactive access to sales information.

### Questions the analysis is intended to support

- How are sales performing against the target?
- How does sales performance change over time?
- How are sales distributed geographically?
- How do product categories compare on profitability?
- How can users move from summary information to more detailed analysis?

## Report at a glance

The supplied report screenshot and PBIX indicate an overview focused on:
- Total sales and sales target
- Sales performance over time
- Sales by continent
- Profit margin by product category

The PBIX is the source of truth for the exact report visuals and calculations. This README deliberately does not invent DAX expressions, relationship cardinalities, or transformation steps that have not been verified from the model.

## Tools and technologies

| Tool / concept | Role in the workflow |
|---|---|
| Power BI Desktop | Data modelling, calculations, and report authoring |
| Power Query Editor | Connecting to, shaping, and preparing source data |
| DAX | Measures, calculated columns, and time-based calculations |
| Power BI Service | Publishing and consuming reports |
| AdventureWorks data | Scenario dataset used for sales analysis |

## Repository contents

```text
sales-analysis-powerbi-dashboard/
├── README.md
├── Sales Analysis.pbix
└── documentation/
    ├── 01-project-and-workflow.md
    ├── 02-data-preparation.md
    ├── 03-data-modeling.md
    ├── 04-dax-reference.md
    ├── 05-report-development.md
    ├── 06-publishing-and-security.md
    └── 07-maintenance-and-learning-log.md
```

## End-to-end workflow

1. **Understand the business request** — define the questions, required detail, and intended users.
2. **Acquire and inspect data** — identify the source files, fields, data types, and relevant business meaning.
3. **Prepare data in Power Query** — connect, inspect, transform, combine, and load the queries.
4. **Build the data model** — organize facts and dimensions, configure relationships, and create useful hierarchies.
5. **Create calculations with DAX** — distinguish calculated columns from measures and add business calculations and time intelligence.
6. **Build the report** — select visuals that answer the questions and configure filters, interactions, tooltips, and navigation.
7. **Publish and manage access** — understand the Power BI Service workflow, workspaces, and row-level security concepts.

## Documentation guide

| File | What it contains |
|---|---|
| [Project and workflow](documentation/01-project-and-workflow.md) | Scenario, requirements, lifecycle, and scope |
| [Data preparation](documentation/02-data-preparation.md) | Source queries, Power Query workflow, merge, append, and refresh |
| [Data modeling](documentation/03-data-modeling.md) | Dimensional modelling, relationships, hierarchies, and model hygiene |
| [DAX reference](documentation/04-dax-reference.md) | DAX concepts and a reusable measure documentation template |
| [Report development](documentation/05-report-development.md) | Visuals, slicers, tooltips, drill-down, drill-through, and design |
| [Publishing and security](documentation/06-publishing-and-security.md) | Power BI Service, dashboards, bookmarks, and RLS concepts |
| [Maintenance and learning log](documentation/07-maintenance-and-learning-log.md) | How to maintain this repository and record future changes |

## Important documentation convention

The course transcript describes a broad Power BI workflow. Not every topic in the course should automatically be interpreted as implemented in this particular PBIX. Where a feature or formula has not been independently confirmed in the report, the documentation describes it as a workflow concept or a verification item rather than claiming it is complete.

When extending this project, update the relevant documentation with:
- The actual source column/table names
- The exact Power Query Applied Steps
- The actual relationship columns and cardinalities
- The exact DAX formula copied from the model
- The visual fields, filters, and interactions used
- Any assumptions, issues, and fixes

## Working with the PBIX

Open `Sales Analysis.pbix` using Power BI Desktop. If the file requests a data-source location or credentials, update the source settings to match the location of the data files available to you. The transcript describes the use of separate dimension and sales source files; those source files are not included in this repository.

## Reference material

The project workflow is documented from the supplied course transcript. The transcript itself is not redistributed in this repository. The PBIX file is included as the working report artifact.

---

**Status:** Working project documentation. Update this README as the report is inspected, refined, and extended.
