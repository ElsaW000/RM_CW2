# COMP4037 Coursework 2: Multivariate Data Visualization

This project presents a multivariate visualization analysis of environmental impacts across various diet and demographic groups, using interactive radar charts and treemaps.

---

## 📊 Visual Design Types

- **Radar Chart**: Comparing multiple environmental indicators across gender, age group, and diet type.
- **Treemap**: Showing variability (standard deviation) in environmental impact indicators, with a hierarchical structure.

---

## 🛠 Tool Used

- Python with Plotly (interactive HTML exports)

---

## 🧪 Variables & Dimensions

- **Diet Groups**: Meat, Meat50, Meat100, Fish, Vegan, Veggie
- **Demographics**: Gender (Male/Female), Age Group (20–79)
- **Environmental Indicators**: GHG Emissions, CH4, N2O, Land Use, Water Use, Water Scarcity, Eutrophication, Acidification, Biodiversity

---

## 🧭 Visual Mappings

| Visual | Size | Color | Hierarchy |
|--------|------|-------|-----------|
| Treemap | Number of participants | Standard deviation (SD) | Gender → Age → Diet |
| Radar | Environmental indicator score | Gender color | Subplots by diet |

---

## 📌 Unique Observation

> **Meat100** diet group consistently exhibits the **highest variability** across environmental indicators, especially in CH₄, Land, and Water Scarcity — suggesting potential presence of outliers or inconsistency within this group.

---

## 📁 File Structure

| File | Description |
|------|-------------|
| `radar_chart_interactive_optimized.html` | Radar chart: environmental impact by diet × gender × age group (with dropdown selector) |
| `all_treemaps_combined.html` | Combined view of all treemap SD charts |
| `treemap_sd_ghgs.html` | SD of GHG emissions |
| `treemap_sd_ghgs_ch4.html` | SD of CH4 emissions |
| `treemap_sd_ghgs_n2o.html` | SD of N2O emissions |
| `treemap_sd_land.html` | SD of land use |
| `treemap_sd_watscar.html` | SD of water scarcity |
| `treemap_sd_watuse.html` | SD of water use |
| `treemap_sd_eut.html` | SD of eutrophication |
| `treemap_sd_acid.html` | SD of acidification |
| `treemap_sd_bio.html` | SD of biodiversity |
| `Results_21Mar2022.csv` | Source dataset |
| `visual_code.py` / `.ipynb` | Code to generate the visualizations |

---

## 🔗 URLs

- **User-Interaction HTML file**: See files in the `html` folder
- **Source code**: See `.py` or `.ipynb` file in this repo

---

## 📦 Data Preparation Notes

- Original CSV cleaned and reshaped to long-form using `pandas.melt()`
- Standard deviation (`sd_*`) computed for each gender × age × diet combination
- All visualizations generated using Plotly and exported as standalone HTML

---

*Created for COMP4037: Research Methods – Data Visualization Coursework (University of Nottingham)*
