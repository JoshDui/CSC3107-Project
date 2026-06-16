# CSC3107 CO2 Visualization Redesign

This project redesigns the Reuters Graphics visualization "Who is the biggest polluter of carbon dioxide?" using the Our World in Data CO2 dataset.

## Project question

The main claim is that the answer to "Who is the biggest polluter?" changes depending on the metric used:

- annual territorial CO2 emissions
- cumulative territorial CO2 emissions
- territorial CO2 emissions per capita
- consumption-based CO2 emissions per capita

## Directory structure

- `data/raw/`: original downloaded OWID data files
- `data/cleaned/`: generated cleaned data used by the redesign
- `figures/`: generated chart exports
- `notes/`: check-in notes and design planning
- `references/`: source and citation notes
- `co2_redesign.qmd`: reproducible import, cleaning, and visualization pipeline

## Reproduce

Render the analysis from the project root:

```powershell
quarto render co2_redesign.qmd
```

The QMD reads `data/raw/owid-co2-data.csv`, writes cleaned CSV files to `data/cleaned/`, and exports the draft small-multiple chart to `figures/`.

`data/raw/owid-co2-data.json` is excluded from git because it exceeds GitHub's 100 MiB file limit. The tracked CSV is the raw dataset used by the reproducible pipeline.
