# Agent log

Add a dated entry each time you work with your AI coding agent, with the newest entry at the bottom. Each entry records what you asked the agent, what it produced, and what you checked or changed. Paste your key prompts in exactly as you typed them. Include at least one time the agent got something wrong, and how you caught it.

Copy this outline for each entry:

```markdown
## YYYY-MM-DD: What you worked on

- **Asked:** "Paste your prompt here."
- **Agent produced:** What it made or changed.
- **Checked or changed:** How you checked it, and what you fixed.
```

## 2026-11-20: Median price chart above the city table

- **Asked:** "Read AGENTS.md and docs/data_description_sheet.md first. Then add a horizontal bar chart of the median sale price for each city above the table on index.html. Keep the table and the $10,000 rule as they are." Then: "Open a pull request into main"
- **Agent produced:** It found that index.html was still the placeholder, with no table and no $10,000 rule, and asked before building. After approval it replaced index.html with a page that loads the CSV, leaves out sales under $10,000, and shows a horizontal bar chart of median sale price by city above a table of sales counted and median price. It also added the rule and figure definitions to the README's Data notes.
- **Checked or changed:** The agent checked the 18 medians and counts against a separate query on the SQLite file, and they matched. Its first version of the chart shrank the text too small to read on a phone; it caught this in a phone-width screenshot and changed the chart to draw at the screen's real width. Opened the website in a tab on browser to ensure that it was indeed readable for a website user. 

## 2026-11-20: Turning on GitHub Pages and filling in the README

- **Asked:** Pasted the README as it appeared on GitHub, then chose the answers to the agent's questions: title "Home Prices in College Towns USA (Declan's Site)", purpose "Compare prices across towns", and "Alone, delete section".
- **Agent produced:** Explained that the first publish failed because GitHub Pages was not turned on, and how to turn it on in the repository's Settings (not the account Settings). After the pull request was merged, it reran the publish workflow, which succeeded. It then filled in the README title, purpose, live site address and tools, and removed the finished "Start here" section and the "Who did what" section. Checked to see that the coding agent's work on adjusting the README tab was successful in meeting requirements. 
