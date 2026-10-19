# A/B Test Analysis

**Status:** 🚧 In progress

## Business question
Did the new campaign/design actually improve conversions, or is the difference just noise?

## Data
- **Source:** [e.g. Marketing A/B Testing or Cookie Cats on Kaggle]
- **Size:** [users per group]
- **Checks done:** [group balance, duplicates, sample ratio]

## Tools
R · tidyverse · ggplot2 · Quarto

## Approach
1. Validated the experiment setup (group sizes, randomization)
2. Compared conversion rates between control and treatment
3. Ran a [two-proportion z-test / chi-square test] and calculated the confidence interval
4. Estimated effect size and statistical power
5. Wrote up the result in a Quarto report (`analysis.qmd`)

## Key insights
- Control conversion: [x%], treatment: [y%]
- Difference: [z points], p-value [p], 95% CI [low, high]
- [Plain-English conclusion: significant or not, and why]

## Recommendation
[e.g. "Roll out the new design, expected lift of ~X conversions per 10,000 visitors."]

## Links
- 📄 Published report: [Quarto Pub or GitHub Pages link]
- 💻 Source: [`analysis.qmd`](./analysis.qmd)

## Reproduce it
```r
install.packages(c("tidyverse", "broom"))
quarto::quarto_render("analysis.qmd")
```

## Repo structure
```
data/          dataset or download link
analysis.qmd   full report with code
```
