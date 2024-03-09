# DEMO

This is the description!

# Deduplication Challenge

This repository tracks the codes for the data deduplication challenge hosted by the Jožef Stefan Institute for Eurostat.

The main file is a Jupyter notebook that calls all other methods: [`main.ipynb`](main.ipynb).

## Dataset Overview

The dataset made available by Eurostat includes the following fields:

- **ID**: The unique OJA identifier, attributed by the Organisation committee.
- **Job title**: The title of the job, retrieved directly from the website.
- **Job description**: The description of the online job advertisement, retrieved directly from the website.
- **Job location**: The place where the job is to be held, extracted automatically from the job description by the WIH.
- **Country ID**: The country ID of the job position derived from the job location.
- **Company name**: The name of the company that is hiring, extracted from the job description.
- **Advertisement retrieval date**: The date (day, month, year) when the job advertisement was retrieved by the web bots of the WIH.

### Types of Duplicates

The dataset contains the following types of duplicates:

- **Full duplicates (or exact duplicates)**: Identical job advertisements in every aspect.
- **Semantic duplicates**: Advertisements for the same position, differing in wording or language.
- **Temporal duplicates**: Semantic duplicates with different advertisement retrieval dates.
- **Partial duplicates**: Advertisements describing the same position but not containing the same characteristics.

Advertisements not fitting into these categories are considered non-duplicates.

## Repository Structure

- [`data`](data/): Contains all input, intermediate, and output data.
- [`src`](src/): Contains all the source code.
- [`tests`](tests/): Contains the unit tests.
- [`assets`](assets/): Contains details of our methodology for ensuring reproducibility.
- [`main.ipynb`](main.ipynb): A wrapper Jupyter notebook to call all functions and build the final dataset.
- [`requirements.txt`](requirements.txt): Contains the project's requirements.

## Authors

- Jannic Cutura
- Dimitrios Petridis
- Stefan Pasch
- Charis Lagonidis


