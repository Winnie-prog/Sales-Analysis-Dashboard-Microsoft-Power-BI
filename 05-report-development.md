# 05 — Report development and visualization

## Purpose

This note records the report-building techniques covered in the course and the analytical role of the visuals in the Sales Analysis report.

## Report questions and visual roles

The supplied dashboard view indicates these main reporting elements:

| Reporting element | Analytical purpose |
|---|---|
| Total Sales KPI/card | Show the headline sales value |
| Sales Target KPI/card | Provide a target for comparison |
| Sales trend over time | Show how sales change across reporting periods |
| Sales by continent | Compare geographical sales distribution |
| Profit margin by product category | Compare profitability across product categories |

Confirm exact visual types, fields, filters, and measure names in the PBIX before treating this table as a complete visual specification.

## Visual types covered in the course

The transcript walks through:
- Clustered column chart
- Clustered bar chart
- Line chart
- KPI visual
- Card visual
- Slicers

Choose a visual based on the question and the comparison it needs to communicate, not simply because the visual is available.

## Filters and slicers

Slicers provide report users with a visible way to filter data. When adding one, document:
- Field used
- Available values
- Single-select or multi-select behaviour
- Whether it affects all visuals or only selected visuals
- Default selection, if any

## Visual interactions

Power BI visuals can interact through cross-filtering and cross-highlighting. Review Edit interactions to ensure selections produce the intended result and do not unintentionally hide relevant information.

## Drill-down and hierarchies

Hierarchies allow users to move between levels of detail within a visual. The course also covers building an order-date hierarchy. Confirm which hierarchies are present in the PBIX and record their level order.

## Drill-through

Drill-through provides navigation from a summary visual to a detail page filtered by the selected data point. Record:
- Source visual
- Drill-through field(s)
- Destination page
- Whether the destination page is hidden
- Back-navigation behaviour
- Fields and visuals shown on the detail page

## Tooltips

The course covers custom tooltips. A useful tooltip adds context to a data point without forcing the user to leave the page. Record the tooltip page, fields, and measures used.

## Bookmarks and navigation

The course includes bookmarks. Bookmarks can preserve a report view or selection state and can support navigation or show/hide interactions. Record what each bookmark captures and which buttons or visuals invoke it.

## Design review checklist

- [ ] The page has a clear analytical purpose.
- [ ] Titles and labels are understandable.
- [ ] KPI values use appropriate number formats.
- [ ] Visuals answer specific business questions.
- [ ] Colours and formatting are consistent.
- [ ] Slicers and filters behave as intended.
- [ ] Cross-interactions have been reviewed.
- [ ] Drill-down and drill-through work as expected.
- [ ] Tooltips add useful context.
- [ ] The report is readable at typical screen sizes.
- [ ] No visual is included without a clear reason.

## Visual inventory — complete from the PBIX

| Page | Visual | Fields / measures | Filters | Interaction / notes |
|---|---|---|---|---|
|  |  |  |  |  |
|  |  |  |  |  |
