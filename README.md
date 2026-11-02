# portfolio-tracker

A single-page HTML app for tracking the progress and status of delivery workstreams across a portfolio.

Open `index.html` in a browser. You do not need a build step or a server. Data is saved in the browser's `localStorage`. Use **Export JSON** and **Import JSON** to back it up or share it.

To try it out, use **Import JSON** to load [`example.json`](./example.json). It's a SpongeBob SquarePants-themed sample portfolio with ratings from June to November 2026, so set the reporting month to November 2026 to see movement.

## Concepts

- **Delivery workstream**: a product or project with a title, one or more owners, and numbers of permanent and contract workers. It also has a summary, a purpose and a set of objectives.
- **Delivery confidence**: a red, amber or green rating recorded for each month.
- **Movement**: worked out by comparing the selected month's rating with the previous month's. It shows as ▲ Improved, ▼ Declined, ▶ No change, or ● New when there is no previous rating.
- **Objectives**: each objective has one or more key results, and each key result has its own progress percentage. An objective's progress is the average of its key results. A workstream's overall progress is the average of its objectives.
- **Monthly update**: for each reporting month, a workstream has a progress update for that month and the work planned for the next month. The details view also shows what was planned last month, so you can compare it with the progress made.
- **Risks / issues / impacts**: each workstream can have any number of entries, each with a description, its mitigations or status, and a red, amber or green rating. They're listed with red first, and the summary panel shows how many red risks and issues there are across the portfolio.