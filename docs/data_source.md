# Data Source and Methodology

## 1. Project Information

| Item | Details |
|---|---|
| Project | India Population Explorer |
| Visualization tool | Tableau |
| Data preparation tool | Microsoft Excel |
| Geographic scope | India |
| Reference year | 2025 |
| Data provider | United Nations Department of Economic and Social Affairs, Population Division |
| Dataset | World Population Prospects 2024 |

## 2. Source of Data

Population data for this project was obtained from the United Nations' *World Population Prospects 2024* (WPP 2024).

The publication provides demographic estimates and projections for countries and areas around the world. The selected dataset is used to explore India's population structure for the 2025 reference year.

**Official source:** https://population.un.org/wpp/

Users should consult the official publication and its technical documentation for detailed definitions, estimation methods, and downloadable datasets.

## 3. Reference Year and Interpretation

The analysis focuses on 2025 population estimates, using 1 July 2025 as the reference date where specified by the selected WPP series.

These figures are estimates produced using demographic methods. They are not a direct count of every person living in India in 2025.

This distinction is important when interpreting the dashboard or comparing its figures with census-based population counts or other published estimates.

## 4. Data Fields

The analysis uses the relevant fields available in the selected source dataset, including the following where present:

- **Location:** country or geographic area.
- **Year:** reference year of the population estimate.
- **Age:** individual age or age category.
- **Sex:** total population, male, or female classification, depending on the selected series.
- **Population:** estimated population value.

The exact field names, units, and category definitions should be checked against the original downloaded dataset.

## 5. Data Preparation Process

Microsoft Excel was used to prepare the source data for visualization in Tableau.

The preparation workflow included the following checks:

1. **Geographic filtering:** select records corresponding to India.
2. **Year filtering:** select the 2025 reference year.
3. **Field selection:** retain the fields needed for population analysis.
4. **Data type checks:** ensure years, age categories, and population values are represented consistently.
5. **Missing-value checks:** identify missing or incomplete values in the selected fields.
6. **Category checks:** review age and sex classifications for consistency.
7. **Validation:** compare totals and component categories where the source definitions make those comparisons valid.

These steps describe the intended preparation workflow. Any additional transformations, exclusions, or corrections should be documented based on the operations actually performed on the final dataset.

## 6. Methodology and Aggregation

The dashboard uses the prepared demographic data to explore population distribution by age and sex.

When interpreting or calculating totals:

- Use the appropriate total-population series when one is supplied.
- Avoid adding total-population records to male and female records, because doing so would double-count the population.
- Avoid summing multiple total rows across age categories or other overlapping categories.
- Confirm whether age records represent individual ages or grouped ranges before aggregating them.
- Preserve the units and definitions supplied by the source.
- Do not combine estimates from different reference years without explicitly accounting for the difference.

Where the source provides both a total-population series and separate male/female series, comparisons should be made using compatible classifications and reference dates.

## 7. Limitations

- Population figures are estimates and may be revised in later UN publications.
- The dataset's methodology may differ from India's official census methodology.
- The dashboard reflects the selected geographic, temporal, and demographic scope.
- Differences in units, age definitions, and sex classifications can affect comparisons with other sources.
- The dashboard is not intended to provide a real-time count of India's population.

## 8. Reproducibility

To reproduce or extend the analysis:

1. Visit the official UN World Population Prospects website.
2. Obtain the relevant WPP 2024 population dataset.
3. Select the same geographic coverage, reference year, and demographic series.
4. Apply the documented data preparation and validation steps.
5. Load the prepared data into Tableau.
6. Recreate or update the dashboard using compatible field definitions.

The exact source download, dataset version, and final field names should be retained with the project files wherever licensing and file-size constraints permit.

## 9. Attribution

Source: United Nations, Department of Economic and Social Affairs, Population Division, *World Population Prospects 2024*.

Official website: https://population.un.org/wpp/

This project is an independent educational and portfolio project. It is not an official United Nations publication or an official government population dashboard.
