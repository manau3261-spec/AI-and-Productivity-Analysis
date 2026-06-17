# AI Adoption and Economic Productivity

An econometric analysis of whether AI adoption by firms is linked to labour productivity across European countries — and whether that link survives once a country's wealth is taken into account.

## Research question

Is there a statistically significant relationship between the adoption of artificial intelligence by firms and labour productivity across European countries?

## Key finding

A simple correlation between AI adoption and productivity does exist (r ≈ 0.64), and is statistically significant. But once GDP per capita is added as a control variable, the AI adoption coefficient becomes **non-significant** — most of the apparent relationship reflects a country's overall wealth rather than a distinct effect of AI. This finding holds whether AI adoption is measured by its 2025 level or by its 2024–2025 growth, and is independently confirmed by an unsupervised clustering approach.

## Method

1. Exploratory data analysis (distributions, correlations, pairplots)
2. Two-sample t-test (high vs. low AI adoption countries)
3. Simple linear regression (productivity ~ AI adoption)
4. Multiple regression with GDP per capita as a control variable
5. Model diagnostics (residual normality, homoscedasticity, VIF)
6. Robustness check using AI adoption growth instead of level
7. K-Means clustering for a country typology (exploratory, descriptive)

## Data sources

All data are from official sources — see [SOURCES.md](SOURCES.md) for full details.

| Variable | Source | Year |
|---|---|---|
| Firm-level AI adoption | Eurostat (isoc_eb_ai) | 2024–2025 |
| Labour productivity (GDP per hour worked) | OECD / ILO | 2025 |
| Real GDP per capita | Eurostat (sdg_08_10) | 2023 |

Sample: 31 European countries (EU member states plus Norway, Albania, Bosnia and Herzegovina, Montenegro, Serbia, and Türkiye).

## Files

- `ai_and_productivity_analysis.ipynb` — full analysis (English)
- `analyse_ia_productivite.ipynb` — full analysis (French)
- `dataset_final_en.csv` / `dataset_final_fr.csv` — final merged dataset
- `SOURCES.md` — detailed data sources and methodological limitations

## Tools

Python, pandas, seaborn, statsmodels, scikit-learn

## Limitations

This is a cross-sectional analysis on a small, European-only sample. It cannot establish causality, and the absence of a significant AI effect does not prove AI has no impact on productivity — only that this particular dataset, at this level of aggregation, does not detect one once wealth is controlled for. See the notebooks' conclusion sections for a full discussion.
