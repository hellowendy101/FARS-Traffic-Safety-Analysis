# FARS Traffic Safety Analysis Project


## Overview

This project examines patterns and trends in fatal motor vehicle crashes in the United States using data from the National Highway Traffic Safety Administration's Fatality Analysis Reporting System (FARS). The goal is to identify patterns in the conditions of fatal crashes occur and how these patterns have changed over time. The findings are intended to provide descriptive evidence that may be useful for transportation safety agencies, Departments of Transportation, and transportation planners.

## Policy Context: why this matters?

Fatal motor vehicle crashes remain an important transportation safety issue. Understanding when crashes occur, the factors associated with them, and how crash patterns change over time can help transportation and traffic safety agencies identify how they can improve the areas where they can prevent. 

## Research Questions

### Q1 — Day / Time Pattern（2024）
When do fatal crashes occur most frequently during the week?

### Q2. Weather Pattern（2024）

What weather conditions are most commonly reported among fatal crashes?

### Q3. Change Over Time（2020–2024）

How have the timing patterns of fatal crashes changed from 2020 to 2024?

## Data

The primary data source for this project is the:

**National Highway Traffic Safety Administration (NHTSA) Fatality Analysis Reporting System (FARS)**

FARS is a national census of fatal motor vehicle traffic crashes in the United States.

The project uses FARS National CSV data for **2020–2024**.

Raw data are obtained from the official NHTSA FARS data repository.

## Data Processing

First, collect 2020 -2024 FARS data. 
Second, select the variables that are needed in 2024 FARS data (accident) and clean the datasets for Q1. Use the processed data for Tableau visualizations.
Third, select the variables that are needed in 2024 FARS data (weather) and clean the datasets for Q2. Use the processed data for Tableau visualizations.

Noted: Only variables relevant to the research questions will be retained in the processed datasets.

## Analysis

### Q1 — Timing of Fatal Crashes

The first analysis examines when fatal crashes occur during the week, including:

- Hour of day
- Day of week

### Q2 — Weather Conditions

The second analysis examines fatal crashes across weather conditions, including:

- Clear
- Rain
- Snow
- Fog
- Other weather conditions

### Q3 — Changes Over Time

The third analysis compares fatal crash patterns across 2020–2024.

## Tools

- Python
- Pandas
- Tableau
- GitHub

## Repository Structure

```text
FARS-Traffic-Safety-Analysis/
│
├── README.md
│
├── data/
│   ├── raw/
│   └── processed/
│
├── code/
│
├── tableau/
│
└── documentation/
