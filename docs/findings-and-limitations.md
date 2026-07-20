# Findings and Analytical Limitations

## Evidence visible in the exported dashboard

### Casualties by province

For the selected side-accident view, the supporting table reports:

| Province | Number of casualties |
|---|---:|
| Zuid-Holland | 1,807 |
| Noord-Holland | 1,257 |
| Noord-Brabant | 708 |
| Utrecht | 647 |
| Gelderland | 501 |

These are descriptive counts and are not adjusted for population or traffic exposure.

### Road situation

The exported road-situation summary shows the largest displayed accident count on straight roads, followed by 3-way crossings, roundabouts and bends. The death-ratio axis should be interpreted cautiously because the displayed table rounds several values to two decimal places.

### Accident outcomes

| Accident ending | Casualties | Accidents | Frequency percent |
|---|---:|---:|---:|
| Injury Hospital | 4,125 | 3,577 | 63.88% |
| Injury Misc | 2,014 | 1,881 | 33.59% |
| Lethal | 133 | 112 | 2.00% |
| Injury First-Aid | 34 | 30 | 0.54% |

Hospital-injury outcomes account for the largest casualty count in this exported view.

### Dry-weather accidents by province

The supporting export includes high dry-weather counts in Zuid-Holland (5,387), Noord-Holland (4,535), Noord-Brabant (2,954), Gelderland (2,867) and Overijssel (2,236).

### Intoxication and uninsured vehicles

The exported provincial summary reports the highest displayed values in Zuid-Holland:

- Number intoxicated: 115
- Number uninsured: 3,749

This does not show that the same vehicles or drivers were both intoxicated and uninsured. The two aggregate measures should not be linked at individual level without record-level analysis.

## Limitations

1. **No causal inference:** The project visualises associations and counts; it does not identify causes statistically.
2. **Aggregation:** Province-level measures cannot support conclusions about individual drivers.
3. **Exposure:** Counts are not normalised by population, kilometres driven, traffic volume, registered vehicles or road length.
4. **Missing and unknown categories:** Unknown accident types and weather categories can influence rankings.
5. **Ratio interpretation:** Ratios may be unstable for small groups and should be shown with denominators.
6. **Time coverage:** The report does not clearly establish a time range or analyse long-term trends.
7. **Policy recommendations:** Recommendations should be treated as hypotheses requiring validation from official road-safety data and subject-matter experts.

## Recommended extensions

- Calculate accidents per 100,000 residents and per registered vehicle.
- Incorporate traffic volume and road exposure.
- Analyse monthly and yearly trends.
- Model accident severity using logistic or ordinal regression.
- Test associations with confidence intervals and significance measures.
- Evaluate missingness and unknown categories systematically.
- Add drill-through pages for province and accident type.
- Separate observed findings, interpretation and policy hypotheses in the dashboard narrative.
