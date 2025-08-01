
<img width="1200" height="800" alt="industry_distribution" src="https://github.com/user-attachments/assets/0e841762-3d0c-48d5-bc0d-f55d7b60b56c" />

# SF Social Simulations // SF 20k Humans

This project uses language models to create a detailed social simulation of San Francisco. The goal is to generate a rich dataset of synthetic humans, or "SF citizens," each with a unique identity, background, and daily life within the city. This data can be used for a wide range of urban studies, social science research, and simulation applications.

NOTE: All data in this repo is purely synthetic and any relation to real life people is coincidental. 

## Data Overview

The data for this simulation is stored in this directory and is organized as follows:

- `data/`: This directory contains individual JSON-LD files for each simulated human in San Francisco. The filenames are formatted as `[ID]_[lastname]_[firstname].jsonld`.
- `_schema.json`: This file provides a formal JSON Schema that describes the structure and constraints of the data contained in each human's JSON-LD file. This schema is useful for data validation and for understanding the data model.

## SF Citizen Data Structure

Each JSON-LD file represents a single SF citizen and is structured according to the `schema.org` vocabulary for a `Person`. The data for each human includes a variety of attributes that define their life in San Francisco. Below is a description of the key fields:

- **`@context`**: The JSON-LD context, which is set to `http://schema.org`.
- **`@type`**: The schema type, which is `Person`.
- **`name`**: The full name of the SF citizen.
- **`givenName`**: The first name.
- **`familyName`**: The last name.
- **`jobTitle`**: The individual's profession or occupation.
- **`gender`**: The gender identity.
- **`nationality`**: The nationality.
- **`birthDate`**: The year of birth, which is approximated from the age of the citizen and the current year of the simulation.
- **`educationalCredentialAwarded`**: The highest level of education attained.
- **`homeLocation`**: The simulated location within the world, which for this dataset is "San Francisco, California."
- **`memberOf`**: If applicable, this describes membership in a family unit, including the family name.

### Additional Properties

A significant amount of detail about each SF citizen is stored in the `additionalProperty` array. Each item in this array is a `PropertyValue` object with a `name` and a `value`. This is where the rich, narrative details generated by the language models are stored. The properties include:

- **`race`**: The racial or ethnic background.
- **`religion`**: The religious beliefs or affiliation.
- **`tribe`**: A descriptor for social group or community affiliation.
- **`personality`**: A summary of the individual's personality traits.
- **`industry`**: The economic sector or industry in which the person works.
- **`backstory`**: A narrative account of the individual's life history.
- **`reveries`**: A description of the person's daydreams, thoughts, and inner monologue.
- **`familyRole`**: The role the individual plays within their family structure.
- **`dayPlan`**: A detailed, hour-by-hour plan of the person's activities for a typical day in San Francisco.

## Usage

This dataset can be used for various purposes, including:
- Analyzing demographic patterns in a simulated urban environment.
- Studying the narrative structures of synthetic life histories.
- As input for agent-based models and other urban simulations.
- For developing and testing AI systems that process and understand human life data.

The `_schema.json` file can be used with any JSON Schema validator to ensure that any new or modified data conforms to the expected structure.

## Citation

If you use this dataset in your research, please cite it as follows:

```bibtex
@misc{hollis2025sf20kpersonas,
  author = {Hollis, Luke},
  title = {SF 20k Personas: 20,000 synthetic human profiles of SF citizens},
  year = {2025},
  publisher = {GitHub},
  journal = {GitHub repository},
  howpublished = {\url{https://github.com/lukehollis/sf_20k_personas}},
  institution = {MIT City Science SF Lab}
}
```

## Analysis

Comparing distributions in synthetic dataset to the real US Census data.

<img width="1200" height="800" alt="race_distribution" src="https://github.com/user-attachments/assets/ae9a3a1d-e701-49aa-beed-ff72448183e4" />
<img width="1200" height="800" alt="industry_distribution" src="https://github.com/user-attachments/assets/6690bc58-dc40-4050-bfb3-4bfb5f802e90" />
<img width="1200" height="800" alt="education_distribution" src="https://github.com/user-attachments/assets/91904bbf-2004-462e-a6e2-ba7b8d323325" />
<img width="1400" height="800" alt="education_by_age" src="https://github.com/user-attachments/assets/cd4c45b7-c606-4ffd-88ff-0eae21907ede" />
<img width="1000" height="600" alt="commute_time_distribution" src="https://github.com/user-attachments/assets/e8dbacd0-8f5c-458c-8ab3-df8ec7acaa83" />
<img width="1200" height="800" alt="commute_method_distribution" src="https://github.com/user-attachments/assets/cf98477b-f396-4077-8963-207d704bb872" />

### Backstories and Reveries

Each simulated bay area denizen has backstory memories and anecdotal "reveries," poignant specific memories from their past. 

<img width="1000" height="500" alt="narrative_themes_topic_4" src="https://github.com/user-attachments/assets/d3d25adb-b6aa-473d-ade4-7536105876db" />
<img width="1000" height="500" alt="narrative_themes_topic_5" src="https://github.com/user-attachments/assets/a2900afa-e35e-48ca-87c4-b114edbe55d2" />
