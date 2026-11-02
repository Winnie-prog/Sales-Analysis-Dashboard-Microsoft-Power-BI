# 07 — Maintenance and learning log

## How to use this repository

Treat this repository as a working technical notebook, not a one-time project announcement.

Whenever the PBIX changes, update the relevant documentation file. Record what changed, why it changed, and how the result was validated.

## Change log

| Date | Area | Change | Reason | Validation |
|---|---|---|---|---|
|  |  | Initial repository documentation | Establish project reference notes | Pending PBIX review |

## Troubleshooting notes

Use this section to preserve solutions to issues so they do not need to be rediscovered.

### Issue template

```text
Date:
Area:
Problem / error:
What caused it:
Steps taken to investigate:
Solution:
How the solution was verified:
Related query / table / measure / visual:
```

## Learning notes

### Power Query
- What transformation was difficult?
- What did the Applied Steps reveal?
- What would be reusable in another project?

### Data modeling
- Which relationship required the most thought?
- Were any keys duplicated or missing?
- How did the model affect filter behaviour?

### DAX
- Which measure was created?
- What did the formula teach you?
- How did filter context change the result?

### Reporting
- Which visual best answered the business question?
- Which interaction improved exploration?
- What design change improved clarity?

### Power BI Service
- What publishing or refresh issue occurred?
- How were permissions or roles tested?

## Future improvements

Add items here only when they are relevant to the actual report:

- [ ] Inspect the PBIX model and fill in the model inventory.
- [ ] Copy exact DAX formulas into the DAX reference.
- [ ] Record the actual Power Query Applied Steps.
- [ ] Document each report page and visual.
- [ ] Validate report totals against the source data.
- [ ] Record refresh and publishing settings, if configured.
- [ ] Test any RLS roles before describing them as active.

## Reference discipline

When a detail is not confirmed, mark it as **To verify** rather than guessing. This keeps the repository useful and trustworthy as a technical reference.
