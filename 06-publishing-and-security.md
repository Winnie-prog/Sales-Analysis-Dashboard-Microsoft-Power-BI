# 06 — Publishing and security

## Purpose

This note records the Power BI Service topics covered in the course and provides a checklist for publishing and managing access.

## Publishing from Power BI Desktop

The course covers publishing a completed PBIX report to the Power BI Service.

Before publishing:
- Save the PBIX file.
- Confirm that the report opens and refreshes as expected.
- Review the data source settings.
- Check that the report does not expose information that should not be shared.
- Confirm the intended workspace.

After publishing, verify that the report and its associated semantic model are available in the selected workspace.

## Report and semantic model

A published solution includes:
- **Report:** the interactive visual presentation.
- **Semantic model:** the data, relationships, and calculations used by the report.

Keep these concepts distinct when documenting updates and refresh issues.

## Power BI Service consumption

The course introduces the Power BI Service reading experience and further service capabilities. When documenting actual use, record:
- Workspace name
- Report name
- Semantic model name
- Intended audience
- Refresh method and schedule, if configured
- Any source credentials or gateway dependency
- Known access limitations

## Dashboards

The course includes building a dashboard in the Power BI Service. A dashboard is a service feature that can bring together pinned content for monitoring. It is distinct from a report page in Power BI Desktop.

Document which report visuals or pages are pinned and why they are useful for monitoring.

## Bookmarks

Bookmarks are also covered as a report interaction and navigation technique. Record the purpose of each bookmark and the view state it captures.

## Row-level security (RLS)

The course introduces creating row-level security roles. RLS restricts which rows a user can see based on the role and identity mapping configured for the model.

When implementing RLS, document:
- Role name
- Table(s) with filters
- Filter expression
- Intended user/group assignment
- How the role was tested
- Whether users are assigned through the Power BI Service

Do not assume RLS is active in the supplied PBIX without checking its role definitions and testing the published report.

## Publishing and access checklist

- [ ] Correct workspace selected.
- [ ] Data source settings reviewed.
- [ ] Refresh tested.
- [ ] Report and semantic model names documented.
- [ ] Intended audience identified.
- [ ] RLS roles reviewed, if required.
- [ ] RLS tested with View as role / appropriate service testing.
- [ ] Workspace and report permissions reviewed.
- [ ] Distribution method documented.
