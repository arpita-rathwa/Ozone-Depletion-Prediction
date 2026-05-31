# 🌍 Ozone Depletion Prediction

> Predicting stratospheric ozone column values using data-driven ML — with SHAP explainability and scenario analysis for policy planning.

---

## Problem Statement

The stratospheric ozone layer is Earth's primary shield against UV-B and UV-C radiation. Despite the 1987 Montreal Protocol phasing out the most harmful Ozone Depleting Substances (ODS), recovery is non-linear and remains threatened by illegal production, climate feedback loops, and geopolitical disruptions.

Existing atmospheric models rely on complex physicochemical simulations that are computationally expensive and cannot easily incorporate socioeconomic uncertainty. This project fills that gap with an interpretable, data-driven ML pipeline.

---

## Technical Scope

### Task Type
- **Multi-output regression** — predicting future ozone column values across multiple atmospheric zones simultaneously

### Data Sources
- NASA observational data (stratospheric ozone measurements)
- NOAA atmospheric records
- 14 custom-engineered socioeconomic and environmental uncertainty parameters (covering pandemics, economic crises, wars, illegal ODS manufacturing)

### Feature Engineering
- **Time-lag features** — capturing the delayed stratospheric response to surface-level ODS emissions (emissions today affect ozone months to years later)
- ODS production and emission trend features per substance class (CFCs, HCFCs, HFCs, etc.)
- Socioeconomic disruption indicators encoded as uncertainty parameters

### Modelling Challenges
- Non-linear recovery dynamics post-Montreal Protocol
- Long lag structures between surface emissions and upper-atmosphere impact
- Incorporating black swan disruptions (COVID, geopolitical shocks) into a continuous regression framework
- Multi-output prediction requiring correlated target handling

### Explainability
- **SHAP (SHapley Additive exPlanations)** — quantifying which ODS substances and socioeconomic conditions drive ozone column changes the most
- Feature importance ranking across substances (CFCs vs. HCFCs vs. emerging compounds)

### Scenario Analysis
- Policy planning under alternative futures — e.g., full compliance vs. continued illegal production vs. accelerated phase-out
- Counterfactual predictions comparing trajectories under different ODS emission assumptions

---

## ML Axes

| Axis | Detail |
|---|---|
| Learning Paradigm & Training Regime | Supervised — trained from scratch on observational data |
| Scope & Complexity | Multi-output regression · Classical to ensemble ML |
| Data Modality | Tabular + time series |
| Explainability & Impact | High — SHAP-driven, interpretable, policy-facing |

---

## To Be Added
- [ ] Framework & libraries used
- [ ] Model architecture and selection rationale
- [ ] Evaluation metrics and results
- [ ] Dataset details and preprocessing steps
- [ ] SHAP plots and scenario analysis outputs
