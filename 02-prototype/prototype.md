# Prototype · Juno

> Module 2 · Prototype the Idea Worth Building.
> Prototype skill created to make building replicable: https://github.com/pali-lespaul/juno-pm/blob/main/01-prompting/prototype-builder-skill.md
> Task we aim for: Build Seven-day feedback digest: a single screen where a PM can review what happened across Slack, Jira, and support tickets during the past week, synthesized into themes.

**Who's using it: **
- Product manager "on-duty" - each week on Monday morning 9:00AM CET, a single PM is selected to go through Slack channel "#customer-feedback-nov19" and summarize tickets and process them for the rest of the team. In case some feedback is unclear, they follow up with customer. They need to understand which feedback is related to bugs, which feedback is feature requests and what part of the product is it related to. They also need to make sure that feedback that is related to top priorities is processes first so it can influence GA.

**Where PM will see output of the Seven-day feedback digest: **
- Directly in Slack. We will use agent to process the feedbacks and share a message in Slack with summary of the tickets and recommended actions.

**What it takes off the plate for PM:**
- A need to go ticket by ticket. We will compile main problems and feedback into categories, flag most important areas to act on and suggest next actions.

  
## Prototype link
https://pali-lespaul.github.io/juno-pm/02-prototype/
_____

## What it demonstrates

It should show how the output will be visible in Slack application. 

_____

## Debrief

- **What worked:** Clearly showed the aggregation from different tools (Slack, Jira, Genesys) + impacted customers and their ARR. 
- **What broke / felt like a toy:** It was too busy - too much information, hard to read. Also the Slack feel was not there.
- **What I'd change next pass:** Provide more information on formatting - to feel more text-based like in Slack. 
