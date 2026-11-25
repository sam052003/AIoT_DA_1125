# 04-experiment Specification

## Purpose

Defines the IEEE ICEIB formatting, Phase W1 empirical data audit reporting, dual-track evaluation protocol, scientific honesty guardrails, and 2020 A–Z SOP (`Q`–`V`) requirements for Section IV (`ICEIB paper/04-Experiment.tex`).

## Requirements

### Requirement: Section IV Experiment Q–V Structure and Empirical Honesty Guardrail
The file `04-Experiment.tex` SHALL follow the `Q` through `V` progression of the 2020 A–Z SOP (`Q` Quality and Quantity Metrics, `R` Related Methods to Compare, `S` Simulation Setup, `T` Tuning & QC Parameters, `U` Useful Phase W1 Empirical Results, and `V` Verify Effectiveness & Scientific Honesty Boundary).

#### Scenario: Verifying empirical W1 data and scientific honesty in 04-Experiment.tex
- **WHEN** `04-Experiment.tex` is checked against `docs/w1-data-integration.md`
- **THEN** it presents `Q` (Track A MAE/RMSE/Skill/regret & Track B tool/citation/rule/degradation/latency metrics), `R` (Persistence & 24h Seasonal Naive vs. Ridge/RF/XGBoost; Rule-Only vs. Agent+ML+Rules), `S` (6 Taichung stations, 70/15/15 split, rolling-origin, 30 Track B cases `B1`–`B6`), `T` (`dedup_identical`, `MAX_VALID_PM25_UG_M3 = 1000.0`, `reconstructed_from_observed_at`), `U` (Table IV live snapshot and Table V 123,055-hour inventory with exact SHA256 prefixes), and `V` (Table VI dual-track matrix with explicit scientific honesty that W2–W6 ML/Agent scores are not pre-claimed)
