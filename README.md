# Traffic Safety and Fatal Motor Vehicle Crashes

## Overview

This project examines patterns and trends in fatal motor vehicle crashes in the United States using the National Highway Traffic Safety Administration's (NHTSA) Fatality Analysis Reporting System (FARS).

The project focuses on when and where fatal crashes occur and how these patterns have changed over time. The analysis is intended to provide descriptive evidence that may be useful for transportation safety agencies, transportation planners, and policymakers when identifying patterns that warrant further attention.

## Research Questions

The project is organized around three questions:

1. **When do fatal crashes occur most frequently during the week?**
   - Examines fatal crashes by day of the week and hour in 2024.
   - Identifies periods with particularly high numbers of fatal crashes.

2. **How does the burden of fatal crashes vary across states?**
   - Compares states using fatal crashes per 100,000 residents in 2024.
   - Uses 2024 state population estimates to provide population-adjusted comparisons.

3. **How have the timing patterns of fatal crashes changed from 2020 to 2024?**
   - Compares the peak hour for fatal crashes across five years.
   - Examines whether the share of annual fatal crashes occurring during the peak hour changed over time.

## Data

### Fatality Analysis Reporting System (FARS)

The primary dataset is the **NHTSA Fatality Analysis Reporting System (FARS)**.

FARS is a census of fatal motor vehicle traffic crashes in the United States. The project uses the national FARS accident-level data for:

- 2020
- 2021
- 2022
- 2023
- 2024

The primary file used in the analysis is `accident.csv`.


### Population Data

For the 2024 state-level analysis, 2024 state population estimates from the U.S. Census Bureau are used to calculate fatal crashes per 100,000 residents.

## Key Measures

### Fatal Crashes

Fatal crashes are counted using the number of records in the FARS accident-level dataset.

### Fatal Crashes per 100,000 Residents

For the state-level analysis:

\[
\text{Fatal Crashes per 100,000 Residents}
=
\frac{\text{Fatal Crashes}}{\text{Population}}
\times 100,000
\]

This measure adjusts the number of fatal crashes for differences in state population.

## Key Findings

### When

Fatal crashes are concentrated during evening and nighttime hours, with several of the highest-count day-hour combinations occurring on Friday and Saturday.

In 2024, the five highest-count day-hour combinations were:

- Saturday, 8:00–8:59 PM — 420 crashes
- Saturday, 11:00–11:59 PM — 414 crashes
- Saturday, 9:00–9:59 PM — 394 crashes
- Saturday, 10:00–10:59 PM — 390 crashes
- Friday, 9:00–9:59 PM — 386 crashes

Four of the five highest-count combinations occurred on Saturday.

### Where

After adjusting for population, the states with the highest fatal crash rates in 2024 were:

1. Mississippi — 23.04 fatal crashes per 100,000 residents
2. New Mexico — 17.74
3. Arkansas — 17.71

These measures represent fatal crashes relative to state population and should not be interpreted as a measure of driving risk because they do not account for traffic exposure such as vehicle miles traveled.

### Over Time

The peak hour for fatal crashes changed over the 2020–2024 period:

- 2020: 6:00–6:59 PM
- 2021: 6:00–6:59 PM
- 2022: 9:00–9:59 PM
- 2023: 8:00–8:59 PM
- 2024: 8:00–8:59 PM

Despite these changes, the share of fatal crashes occurring during the peak hour remained relatively stable, ranging from approximately 5.93% to 6.16% of annual fatal crashes.

## Repository Structure

```text
FARS-Traffic-Safety-Analysis/
│
├── code/
│   └── data_cleaning_code.ipynb
│
├── data/
│   ├── raw/
│   │   ├── 2024POP.xlsx
│   │   └── README.md
│   │
│   └── processed/
│       ├── Q2.csv
│       └── Q3_peak_hour_2020_2024.csv
│
├── documentation/
│   └── Xiao_ProjectProposal_Fatal_Crash.pdf
│
├── tableau/
│   ├── Sheet 1.png
│   ├── Sheet 2.png
│   ├── Sheet 3.png
│   └── Traffic Safety Project Tableau workbook
│
├── .gitignore
└── README.md
