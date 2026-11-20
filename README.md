# Home Prices in College Towns USA (Declan's Site)

## What this site is for

**Question:** How do typical home prices compare across 18 college towns in the United States?

**Audience:** People deciding where to buy or rent near a university campus, such as students, university staff and families.

The home page shows the median sale price for each city as a bar chart, with a table of the same figures below it.

## Live site

https://dpcolleran.github.io/DeclanNewRepository11-19/

## Data notes

- **The $10,000 rule.** Sales under $10,000 are left out as implausible prices (40 of 35,442 sales, including one at $0). Sales over $5,000,000 are kept: the site reports medians, which a few very high prices barely move.
- **Median sale price by city** (chart and table on the home page): the median `sale_price` of the sales that pass the $10,000 rule, grouped by `city` and `state`. With an even number of sales it is the average of the two middle prices, rounded to the dollar. The page computes it from `data/college_town_home_sales.csv` in the browser each time it loads.
- **Sales counted**: the number of sales in that city that pass the $10,000 rule.
- These medians can differ slightly from the description sheet's table, which leaves out only sales under $1,000 (for example, Ann Arbor is $572,000 here and $571,000 there).

## Tools we used

- **AI coding agent:** Claude Code.
- **Site:** plain HTML, CSS and JavaScript, with no libraries. The chart is drawn as SVG by the page's own script.
- **Checking numbers:** the medians and sales counts were checked against a separate query on `data/college_town_home_sales.sqlite`.
- **Hosting:** GitHub Pages, published by the GitHub Actions workflow in `.github/workflows/pages.yml`.

## Citation

College-town home sales dataset, version 1.0 (2026). University of Illinois-Deloitte Foundation Center for Business Emerging Technologies. Data collected March 2026.
