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
- **Code**: Jupyter Notebook (`.ipynb`) please open `Data_Visulaisation.ipynb` in google colab or click on link here (https://colab.research.google.com/drive/1CfekAZRX-vsvNaJPPBKgNWJGIjqThW04?usp=sharing)
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

## Tools and Libraries / Dependencies
Anyone trying to clone this repository perform 
`pip install -r requirements.txt`
The following were used to generate the visuals 
- Pandas Version: 2.2.2
- Seaborn Version: 0.13.2
- Matplotlib Version: 3.10.0
- Numpy Version: 2.0.2
- Scikit-learn Version: 1.6.1
- Plotly Version: 5.24.1

---

## Key Features
- **Diet Categories**: Vegan, Vegetarian, Fish-eater, Meat-eater (meat50 and meat100 merged into Meat)
- **Normalization**: Environmental variables scaled to [0,1] using `MinMaxScaler`
- **Layperson-friendly Labels**: Technical column names renamed for clarity
- **Interactivity**: Sunburst and Radar charts are fully interactive (available as `.html` files)

---

 ## Observations
- Meat-heavy diets (even when merged) show consistently higher environmental costs across all indicators (red zone in heatmap and full radial coverage in radar).
- Fish-based diets, while lower in GHGs, show higher water use and water scarcity footprint, which is a non-obvious insight from the radar chart.
- The sunburst chart reveals that females dominate vegetarian/vegan groups, particularly ages 20-39, indicating demographic shifts in sustainable eating (seen visually in the expanded purple and blue sectors).
--- 
## Running the Code
1. Please open `Data_Visulaisation.ipynb` in google colab or click on link here (https://colab.research.google.com/drive/1CfekAZRX-vsvNaJPPBKgNWJGIjqThW04?usp=sharing)
2. Upload `Results_21Mar2022.csv` to your Colab session.
3. Update the path if necessary:
   ```python
   df = pd.read_csv('/content/Results_21Mar2022.csv')

   ```
4. Run all cells to generate visualizations.

5. (Optional) Export high-resolution PNGs/ html files by uncommenting the provided save commands.

---

## Viewing the Outputs 
- Navigate to the visualisations/ folder.
- For HTML Files (Interactive Charts):
- Download the .html files to your local machine.
- Open them using any web browser (e.g., Chrome, Firefox, Edge).
- The charts are fully interactive (hover, zoom, explore).
- For PNG File (Static Chart):
- The static heatmap is available as a .png file inside the same folder
- The `observations.txt` contains the insights obtained from the graphs present in outputs folder 
---
## Notes
- Bar charts, pie charts, line charts, and bubble charts were avoided as per coursework requirements.

- Advanced designs (hierarchical, normalized, multivariate) were used to maximize insight discovery.
   
