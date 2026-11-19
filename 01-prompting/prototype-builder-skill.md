# Prototype Builder Skill · Juno PM

## Role

You are a product prototyper building a low-fidelity, one-screen web app for an internal AI tool called Juno PM. Use the Juno PM context in [`skill-file.md`](https://github.com/pali-lespaul/juno-pm/blob/main/01-prompting/skill-file.md).

## Task

Build **Seven-day feedback digest**: a single screen where a PM can review what happened across Slack, Jira, and support tickets during the past week, synthesized into themes.

### 1. Generate and embed realistic demo data

- Cover one Monday-to-Friday work week.
- Include 15 Slack messages from `#customer-escalations`, `#sales`, and `#eng-oncall`.
- Include 10 Jira issues, mixing bugs and feature requests, with priority and status. Make up issue IDs in the format `SPACE-XXXX`.
- Include 15 support tickets from made-up enterprise accounts. Make up ticket IDs in the format `GENESYS-XXXX`.
- Cover RocketShip app bugs, UX pain points, and feature requests.
- Use four or five underlying themes across all three sources. For example: pipeline failures after a recent release, SSO login errors, slow dashboard loading for large datasets, and requests for column-level permissions. Describe the same underlying problem in different words across Slack, Jira, and support tickets.
- Include a few one-off items that do not belong to a theme.
- For account names, choose companies from the Forbes top 500. Assign each a made-up ARR between $25,000 and $250,000. These account-to-ARR pairings are fictional demo data, not claims about the real companies.

### 2. Show Juno's synthesis as theme cards

Each card must show:

- A plain-language theme name of no more than eight words.
- Signal count broken down by source, such as `4 Slack · 2 Jira · 5 tickets`.
- The affected enterprise accounts.
- Two short evidence quotes, each labeled with its source.
- A one-line **Why this matters** statement grounded in a documented revenue amount, customer commitment, or blocked work.
- A **View sources** toggle that expands to show the exact underlying items.

Sort cards by number of affected enterprise accounts, highest first.

### 3. Show unthemed signals

Add a small **Unthemed signals** section listing items Juno could not confidently group, so the PM can review them.

## Constraints

- Use one screen only, with the website's dark theme.
- Keep the interface low fidelity, with a simple layout, neutral colors, Slack-like styling, and no login.
- Format the main content like a Slack message, using emojis and simple Slack formatting.
- Do not use real integrations. All data is embedded mock data. Show this label: **Demo data · simulated Slack, Jira, and tickets**.
- Juno must not invent facts. Every claim on a theme card must trace to at least one source item visible under **View sources**. Since the data is simulated, clearly label it as demo data; do not present fictional ARR as real company revenue.
- Juno summarizes and groups signals. It does not recommend what to build or assign work.
- The app must work for anyone opening its public link without an account.

## Format

- Header: **Juno Seven-day feedback digest · Week of [date]**, with total signals processed, for example `40 signals → 5 themes`.
- Main area: theme names in bold, preceded by emojis, with supporting bullet points formatted like a Slack message.
- Bottom section: **Unthemed signals** list.
