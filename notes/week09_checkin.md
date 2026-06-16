# Week 09 Check-In Draft

## Draft design brief

This redesign is intended for climate-policy students and general news readers comparing national responsibility for CO2 emissions. The task is to understand how the answer to "who is the biggest polluter?" changes under different fairness measures: annual territorial emissions, cumulative historical emissions, territorial emissions per capita, and consumption-based emissions per capita. The redesign will use coordinated small multiples, consistent country colors, direct labels, normalized units, and short annotations explaining the limits of each metric.

## Design direction

The project will redesign the Reuters Graphics article "Who is the biggest polluter of carbon dioxide?" Instead of using a dense Sankey-style flow and rotated labels, the new poster will use a 2x2 small-multiple comparison. Each panel will show the same selected countries so readers can compare how rankings and responsibility change when the metric changes.

The working dataset is the Our World in Data CO2 and Greenhouse Gas Emissions dataset. The first reproducible pipeline reads the raw OWID CSV, filters a small comparison set, selects the latest year with complete values for all four metrics, exports cleaned data, and generates a draft chart.

## Questions for instructors

1. Is the four-metric framing sufficiently focused for the poster, or should we reduce it to three metrics to improve readability?
2. Should the European Union be included as a meaningful policy bloc, or should the comparison use countries only?
3. Is consumption-based per-capita CO2 a suitable fourth metric, given that it is available for fewer recent years than territorial emissions?
