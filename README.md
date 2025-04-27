# Interactive-Data-Visualisation
The project visualizes the environmental impacts of different diets (vegan, vegetarian, fish-eater, meat-eater) using the Oxford University dataset. Includes advanced visual designs and a unique observation

# Environmental Impact of Dietary Choices: An Advanced Visual Analytics Report


## Student Information
- **Name**: Fahad Mujawar
- **Student ID**: 20711746
- **Module**: COMP4037 - Research Methods
- **University**: University of Nottingham
- **Date**: April 2025

---

## Overview
This repository contains Python code developed for COMP4037 Coursework 2 (Research Methods).  
The project focuses on visualizing the environmental impact of different dietary groups based on the Oxford University dataset ("Vegans, vegetarians, fish-eaters and meat-eaters in the UK show discrepant environmental impacts" – Scarborough et al., 2023).

The goal was to generate advanced visual designs to uncover non-trivial insights about greenhouse gas emissions, land use, water use, biodiversity impact, and other sustainability metrics across diet types.

---

## Project Structure
- **Dataset Used**: `Results_21Mar2022.csv` (upload manually when running)
- **Environment**: Google Colab
- **Visualizations Produced**:
  - **Sunburst Chart**: Hierarchical distribution by diet, gender, and age group
  - **Heatmap**: Normalized environmental intensity across diet groups
  - **Radar Chart**: Multivariate comparative analysis across environmental metrics

---

## Tools and Libraries
- `Pandas`
- `Seaborn`
- `Matplotlib`
- `Plotly`
- `Scikit-learn`

---

## Key Features
- **Diet Categories**: Vegan, Vegetarian, Fish-eater, Meat-eater (meat50 and meat100 merged into Meat)
- **Normalization**: Environmental variables scaled to [0,1] using `MinMaxScaler`
- **Layperson-friendly Labels**: Technical column names renamed for clarity
- **Interactivity**: Sunburst and Radar charts are interactive

---

## Observations
- Meat-heavy diets consistently show higher environmental harm across all metrics.
- Fish-based diets, while lower in GHG emissions, show higher water use and eutrophication potential.
- Females aged 20–39 dominate vegetarian and vegan groups (based on Sunburst Chart demographic layers).

---



## Running the Code
1. Upload `Results_21Mar2022.csv` to your Colab session.
2. Update the path if necessary in the notebook:
   ```python
   df = pd.read_csv('/content/Results_21Mar2022.csv')
   ```
3. Run all cells to generate visualizations.

4. (Optional) Export high-resolution PNGs by uncommenting the provided save commands.

---
## Notes
- Bar charts, pie charts, line charts, and bubble charts were avoided as per coursework requirements.

- Advanced designs (hierarchical, normalized, multivariate) were used to maximize insight discovery.
   
