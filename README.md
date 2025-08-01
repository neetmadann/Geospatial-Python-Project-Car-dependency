# 🚗 Geospatial Prediction of Car Dependency in England using Urban Form
## 🧠 Overview
This research explores whether **urban form**—the physical layout and structure of built environments—can be used to predict **car dependency** across spatial areas in England. The analysis leverages machine learning to assess how much car ownership is influenced by:

- 🧍 Socio-demographic factors  
- 💷 Socio-economic conditions  
- 🏘️ Urban form characteristics (e.g., building alignment, street openness)

## 🎯 Research Objectives
- Predict car dependency at the **MSOA** level using spatial and tabular data.
- Understand the contribution of **urban form features** to car ownership.
- Support **urban planning** and **transport policy** by identifying car-reducing built environments.

## ❓ Key Research Questions
1. What socio-demographic, economic, and environmental factors best explain car ownership?
2. Can urban form features alone predict car dependency in absence of traditional variables?
3. Do urban form features improve predictions when combined with other variables?

## 🧪 Methodology
- **Data sources** include spatial building/street data and census statistics.
- **Urban form metrics** (68 variables) were generated using Voronoi tessellation with `momepy`.
- **Spatial cross-validation** was performed using K-means clustering and K-fold evaluation.

## 📊 Results Summary

| Model Type               | Accuracy (Lasso) | Accuracy (Random Forest) |
|--------------------------|------------------|----------------------------|
| Traditional Features     | 80%              | 78%                        |
| Urban Form Only          | 81%              | 76%                        |
| All Features Combined    | 81%              | 80%                        |

- **Urban form alone** has strong predictive power (up to 76% accuracy).
- **Top predictors** include Age, Population Density, Cell Alignment, and Income.

## 🧠 Key Findings
- Areas with **modernist, suburban, or rural** urban form (e.g., misaligned buildings, sparse streets) show **higher car dependency**.
- **Dense, walkable** urban environments like **central London** show **lower car use**.
- Urban form can be a **proxy indicator** of transport behavior and planning quality.

## 🧭 Policy Relevance
This research offers insights for:
- **Urban planners** seeking to reduce forced car ownership.
- **Policymakers** developing sustainable transport infrastructure.
- **Local governments** identifying high-dependency areas for targeted investment.

## ⚠️ Limitations
- Data comes from multiple years, creating potential inconsistencies.
- Prediction accuracy may improve with time-aligned datasets.

## 🔮 Future Research
- Separate analysis of **London vs. other regions** to understand unique urban traits.
- Explore **ensemble models** (e.g., combining Lasso and Random Forest).
- Investigate how **urban form redesign** can promote car-free lifestyles.
