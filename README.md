# DS 2500 — Data Wrangling

Coursework notebooks for DS 2500 (Data Wrangling).

## Notebooks

| Assignment | Notebook | Topic |
|---|---|---|
| Module Assignment 1 | [`ModuleAssignment1.ipynb`](notebooks/ModuleAssignment1.ipynb) | Exploratory data analysis: does the share of fatal collisions involving alcohol-impaired drivers vary by U.S. region? |

### Module Assignment 1 — Alcohol-Impaired Fatal Collisions by Region

- **Data:** FiveThirtyEight's `bad-drivers` dataset (one row per state + D.C.), read directly from a raw CSV on GitHub. States are mapped to the four Census Bureau regions.
- **Method:** EDA checklist (shape, head/tail, range checks, external validation), a box plot by region, then a one-way ANOVA after checking normality (Shapiro–Wilk, probability plots) and equal variance (Levene's test).
- **Result:** F = 0.51, p = 0.677 — no statistically significant difference between regions. Roughly 30% of drivers in fatal crashes were alcohol impaired everywhere, so drunk driving looks like a national problem rather than a regional one.

## Running the notebooks

```bash
pip install jupyter pandas numpy matplotlib seaborn scipy
jupyter notebook notebooks/
```

Data is loaded from public URLs, so no local data files are needed.

## A note on AI use

I use [Claude Code](https://claude.com/claude-code) to help manage this repository (organizing files, writing this README, and handling git). All of the code, analysis, and writing inside the notebooks is my own work.
