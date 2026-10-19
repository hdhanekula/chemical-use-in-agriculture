# Agricultural Chemical Use: Identifying Crop Systems for Reduced Chemical Dependence

## MSDS 692 — Data Science Practicum

**Project focus:** Comparing agricultural chemical use in cotton and potatoes using USDA National Agricultural Statistics Service (NASS) 2025 data.

## Project Overview

This project examines reported pesticide-use patterns in cotton and potato production to identify opportunities for further research into integrated pest management (IPM) and lower-chemical agricultural practices.

The analysis focuses on the percentage of planted acres treated with different pesticide categories. It also examines selected reported pest-management practices for potatoes.

The goal is to prioritize research and potential field trials—not to claim that a specific alternative has already been proven effective.

## Research Questions

1. How does pesticide-use coverage differ between cotton and potatoes?
2. Which pesticide categories have the broadest reported coverage in each crop?
3. What pest-management practices are reported in potato production?
4. How can these findings inform future research into integrated, lower-chemical approaches?

## Data Sources

The datasets come from USDA NASS Quick Stats predefined queries for the 2025 Cotton and Potatoes Chemical Use Survey.

| File | Description |
|---|---|
| `cotton_pesticide_use_2025_quickstats.csv` | Cotton pesticide-use estimates |
| `potato_pesticide_use_2025_quickstats.csv` | Potato pesticide-use estimates |
| `cotton_pest_management_2025_quickstats.csv` | Cotton pest-management practices |
| `potato_pest_management_2025_quickstats.csv` | Potato pest-management practices |
| `Agriculture_Chemical_Use_PPT_Aligned_EDA.ipynb` | Exploratory data analysis notebook |

## Exploratory Data Analysis

The notebook follows the descriptive analysis presented in the final PowerPoint:

- Compares herbicide, insecticide, fungicide, and other-chemical coverage between cotton and potatoes.
- Uses percentage of planted acres treated as the primary comparison measure.
- Presents crop comparisons on a common 0–100% scale.
- Summarizes selected potato pest-management practices, including scouting, crop rotation, ground cover or barriers, and equipment cleaning.
- Performs data checks and documents interpretation limitations.

### Key Findings

The rounded crop-level estimates reported in the USDA NASS 2025 highlights are:

| Pesticide category | Cotton | Potatoes |
|---|---:|---:|
| Herbicides | 88% | 90% |
| Insecticides | 39% | 92% |
| Fungicides | 1% | 96% |
| Other chemicals | 54% | 29% |

Reported potato pest-management practices include:

| Practice | Percentage of planted acres |
|---|---:|
| Scouting | 99% |
| Equipment cleaning | 86% |
| Crop rotation | 75% |
| Ground cover or barriers | 79% |

**Interpretation:** Potato production shows broad reported coverage across herbicides, insecticides, and fungicides, making it a useful candidate for further research into integrated pest management. Cotton provides a distinct research pathway, particularly around weed management.

These estimates describe reported use and practice coverage. They do not establish pesticide toxicity, overall risk, or the effectiveness of alternative practices.

## Methods and Limitations

- The primary metric is percentage of planted acres treated because it describes the breadth of pesticide use.
- Application rates, number of applications, and total pounds applied represent different aspects of use and should not be treated as interchangeable measures.
- Pesticide-category percentages can overlap and must not be added together.
- USDA estimates may include suppressed or unavailable values, which must not be interpreted as zero.
- Cotton and potato surveys cover different sets of states.
- The crop-level estimates support descriptive comparisons, not causal conclusions.

A state-level statistical model is a potential next step, not a completed result. State-level estimates, independent sample sizes, missing or suppressed values, and survey precision must be validated before state rankings or regression results are reported.

## Recommendation

Prioritize research into an integrated, lower-chemical pest-management approach for potato systems while evaluating a separate, crop-appropriate weed-management pathway for cotton.

A future field trial should compare the proposed integrated approach with current grower practices and measure chemical use alongside yield, crop quality, pest control, and farm economics. Practices should be tested rather than assumed to be effective substitutes.

## Repository Contents

- **CSV files:** USDA NASS Quick Stats source exports for pesticide use and pest management.
- **Jupyter notebook:** Descriptive EDA aligned with the final presentation.
- **Presentation:** Project findings, recommendations, proposed evaluation design, and limitations.

## References

1. USDA NASS — [2025 Potato Chemical Use Highlights](https://www.nass.usda.gov/Surveys/Guide_to_NASS_Surveys/Chemical_Use/2025_Cotton_Potatoes/ChemHighlights2025PotatoFINAL.pdf)
2. USDA NASS — [2025 Cotton Chemical Use Highlights](https://www.nass.usda.gov/Surveys/Guide_to_NASS_Surveys/Chemical_Use/2025_Cotton_Potatoes/ChemHighlights2025CottonFINAL.pdf)
3. USDA NASS — [2025 Cotton and Potatoes Quick Stats Queries](https://www.nass.usda.gov/Data_and_Statistics/Pre-Defined_Queries/2025_Cotton_Potatoes/index.php)
4. USDA NASS — [Agricultural Chemical Usage: Field Crops Methodology and Data Quality](https://www.nass.usda.gov/Publications/Methodology_and_Data_Quality/Agricultural_Chemical_Usage_-_Field_Crops/index.php)

---

*This project uses observational survey estimates to identify research opportunities. It does not claim that a lower-chemical alternative has already been demonstrated to maintain crop yield, quality, or profitability.*
