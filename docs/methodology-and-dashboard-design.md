# Methodology and Dashboard Design

## Data source

The project used the **Case Study - Dutch Traffic Accidents** dataset available within SAS Viya for Learners. The source contained approximately 57 numeric and categorical variables. The portfolio repository does not redistribute the source dataset.

## Analytical approach

The project used exploratory visual analysis rather than predictive or causal modelling. The workflow was:

1. Review available fields and select variables relevant to accident frequency and severity.
2. Organise the dashboard around accident type as a recurring analytical dimension.
3. Build geographic and comparative visualisations in SAS Visual Analytics.
4. Apply filters for accident type, non-missing values and selected value ranges.
5. Compare observed patterns across provinces, road situations, weekdays, outcomes and weather conditions.
6. Summarise findings in a structured visual report.

## Selected variables

- Type accident
- Number accidents
- Number casualties
- Province name
- Ratio deaths
- Road situation
- Ratio casualties
- Weekday accident
- Accident ending
- Frequency percent
- Weather condition 2
- Number intoxicated (liquor/drugs)
- Number uninsured

## Visual objects

### Geographic casualty map

- **Category:** Province / Province name
- **Measure:** Number casualties
- **Filter:** Accident type
- **Purpose:** Identify provincial differences in casualty counts.

### Road-situation dual-axis chart

- **Category:** Road situation
- **Measures:** Ratio deaths and Number accidents
- **Filter:** Accident type and non-missing values
- **Purpose:** Compare accident volume with severity ratio across road layouts.

### Weekday dual-axis plot

- **Category:** Weekday accident
- **Measures:** Ratio deaths and Ratio casualties
- **Filter:** Accident type and non-missing weekdays
- **Purpose:** Compare weekday variation in two severity measures.

### Accident-outcome bubble plot

- **Category:** Accident ending
- **Measures:** Number accidents, Number casualties and Frequency percent
- **Filter:** Accident type and non-missing outcomes
- **Purpose:** Compare outcome frequency and casualty burden.

### Weather-condition map

- **Category:** Province
- **Group/colour:** Weather condition 2
- **Measure:** Number accidents
- **Filter:** Accident type, non-missing province and weather
- **Purpose:** Show provincial accident counts across weather categories.

### Intoxication and insurance treemap

- **Category:** Province name
- **Measures:** Number intoxicated and Number uninsured
- **Filter:** Accident type and non-missing province
- **Purpose:** Compare two recorded risk indicators across provinces.

## Quality checks for a future rebuild

- Confirm whether measures represent raw counts, frequencies or pre-calculated ratios.
- Verify that filters do not unintentionally exclude valid zero values.
- Compare dashboard totals with exported summary tables.
- Keep unknown categories visible during quality assessment, then explain any exclusions.
- Use clear titles that distinguish counts from ratios.
- Avoid interpreting province-level associations as individual-level relationships.
