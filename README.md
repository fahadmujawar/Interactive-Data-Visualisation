# Environmental Impact of Dietary Choices: An Advanced Visual Analytics Report
## Student Information
- **Name**: Fahad Mujawar
- **Student ID**: 20711746
- **Module**: COMP4037 - Research Methods
- **University**: University of Nottingham
- **Date**: April 2025

---

## Overview
This repository contains Python code and visualization outputs developed for COMP4037 Coursework 2 (Research Methods).  
The project focuses on visualizing the environmental impact of different dietary groups based on the Oxford University dataset ("Vegans, vegetarians, fish-eaters and meat-eaters in the UK show discrepant environmental impacts" – Scarborough et al., 2023).

The goal was to generate advanced visual designs to uncover non-trivial insights about greenhouse gas emissions, land use, water use, biodiversity impact, and other sustainability metrics across diet types.

---

## Project Structure
- **Dataset Used**: `Results_21Mar2022.csv` (upload manually when running)
- **Environment**: Google Colab
- **Code**: Jupyter Notebook (`.ipynb`)
- **Outputs Folder**: `visualisations/`
  - Contains interactive charts (`.html` files)
  - Contains high-resolution static image (`.png` file)
  - Contains `observations.txt` which has the observations saved 

---

## Visualizations Produced
- **Sunburst Chart**: Hierarchical distribution by diet, gender, and age group (interactive).
- **Heatmap**: Normalized environmental intensity across diet groups (static PNG).
- **Radar Chart**: Multivariate comparative analysis across environmental metrics (interactive).

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
- **Interactivity**: Sunburst and Radar charts are fully interactive (available as `.html` files)

---

## Running the Code
1. Upload `Results_21Mar2022.csv` to your Colab session.
2. Update the path if necessary:
   ```python
   df = pd.read_csv('/content/Results_21Mar2022.csv')

   ```
3. Run all cells to generate visualizations.

4. (Optional) Export high-resolution PNGs/ html files by uncommenting the provided save commands.

---
## Notes
- Bar charts, pie charts, line charts, and bubble charts were avoided as per coursework requirements.

- Advanced designs (hierarchical, normalized, multivariate) were used to maximize insight discovery.
   
