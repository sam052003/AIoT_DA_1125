# Spec Delta

## Purpose

Defines the structural, rhetorical (2020 A–Z SOP), technical, and IEEE ICEIB conference formatting requirements for the AirGuard AI academic manuscript (`ICEIB paper/main.tex` and `ICEIB paper/main.txt`) and its Overleaf synchronization.

## ADDED Requirements

### Requirement: IEEE ICEIB Conference Formatting and Section Organization
The manuscript SHALL conform to the IEEE International Conference on Electronic Communications, Internet of Things and Big Data (ICEIB, `www.iceib.asia`) two-column A4 conference format (`\documentclass[conference,a4paper]{IEEEtran}`) with top-level sections ordered as `Abstract`, `Index Terms`, `I. Introduction`, `II. Related Work`, `III. Proposed Design`, `IV. Experiment`, `V. Conclusion`, and `References`.

#### Scenario: Verifying section structure and author order
- **WHEN** the manuscript (`ICEIB paper/main.tex` and `ICEIB paper/main.txt`) is inspected or compiled on Overleaf (`6b064a46a654dfea12d0fd00`)
- **THEN** it lists `Ming-Hsien Tsai (7115056013)` as first author followed by `Hung-Yang Lin (7115056179)` and `Ping-Kun Hsu (8114056002)`, and renders `Abstract`, `Index Terms`, `I. Introduction`, `II. Related Work`, `III. Proposed Design`, `IV. Experiment`, `V. Conclusion`, and `References` (`[1]`–`[24]`) with zero LaTeX errors

### Requirement: Abstract A–F Rhetorical Structure
The `Abstract` SHALL be written as a single coherent paragraph (150–250 words) following the six rhetorical elements of the 2020 A–Z SOP (`A` Motivation, `B` But, `C` Cure, `D` Development, `E` Experiments, and `F` Findings/Expected Outcomes) without fabricating unverified experimental results.

#### Scenario: Auditing Abstract against A–F SOP
- **WHEN** the `Abstract` is evaluated against `myRef/A2Z outline example.pdf`
- **THEN** it includes `A` (WHO 2019 4.2M deaths and MOENV 2019–2025 $\text{PM}_{2.5}$ trend $16.2 \rightarrow 12.8\,\mu\text{g/m}^3$), `B` (status-to-action gap, leakage risks, and LLM AQI/$\text{PM}_{2.5}$ conflation), `C` (AirGuard AI Domain AI Agent), `D` (4 MOENV datasets, 1/3/6h baselines vs. Ridge/RF/XGBoost, 2025 AQI rules, 8-tool ReAct agent, $\mu\text{g}\cdot\text{h/m}^3$ exposure index), `E` (Phase W1 6-station Taichung audit and Track A/B protocol), and `F` (station-scale scope boundary and expected outcomes)

### Requirement: Section I Introduction G–L Rhetorical Structure
Section `I. Introduction` SHALL follow the `G` through `L` progression of the 2020 A–Z SOP (`G` General Current Status, `H` However/Challenges, `I` In Literature taxonomy from old to new and simple to complex, `J` Judgement/SWOT critique, `K` Keypoint & major contributions summary, and `L` List the organization).

#### Scenario: Auditing Introduction against G–L SOP
- **WHEN** Section `I. Introduction` is reviewed against the 2020 A–Z SOP
- **THEN** it systematically presents `G` (global and Taiwan air quality context), `H` (timestamp conflation, zero-imputation fallacy, multi-pollutant AQI vs. single-pollutant $\text{PM}_{2.5}$ divergence, and spatial station-vs-street limits), `I` (literature progression across forecasting, XAI, and tool agents), `J` (SWOT critique of accuracy-vs-decision gap and unconstrained LLM risks), `K` (four numbered contributions), and `L` (paper roadmap for Sections II–V)

### Requirement: Section II Related Work M–O and Deep Research Integration
Section `II. Related Work` SHALL follow the `M` through `O` progression of the 2020 A–Z SOP (`M` Methods across 50% AI Technology and 50% Domain Know-how, `N` New Proposed trend & Deep Research Q1/Q2/Q3 synthesis with the four-stage Research Gap chain, and `O` Organize via a structured SWOT Article Summary Table).

#### Scenario: Auditing Related Work against M–O SOP and 50/50 AI-Domain balance
- **WHEN** Section `II. Related Work` is inspected
- **THEN** it balances `M` (AI time-series validation, M5 baseline rigor, SHAP, ReAct, OWASP LLM01 vs. WHO AQG, concentration-exposure-dose hierarchy, 2025 MOENV AQI rules, and 2026 *BAMS* hourly forecast utility), `N` (5 Core Mindsets, 3 Key Controversies, 10 Deep Questions, and `Existing Research -> Limitations -> Research Gap -> AirGuard AI`), and `O` (Table I comparing references across Problem, Method/Domain, Dataset, Findings, and Limitations)

### Requirement: Section III Proposed Design PA–PM Structure and Three Technical Representations
Section `III. Proposed Design` SHALL follow the `PA` through `PM` progression of the 2020 A–Z SOP and MUST include all three required technical representations: the eight-module architecture (`①`–`⑧`), the fail-closed quality-check flowchart, and line-numbered pseudocode for Algorithm 1 and Algorithm 2.

#### Scenario: Verifying PA–PM elements and three technical representations
- **WHEN** Section `III. Proposed Design` is reviewed
- **THEN** it covers `PA` (Aim), `PB` (MOENV datasets Table II & data contracts), `PC` (Dual-track Official AQI vs. Predicted $\text{PM}_{2.5}$), `PD` (Design paradigm shift), `PE` (Modules `①`–`⑧`), `PF` (mathematical formulations for Persistence, Seasonal Naive, MAE, RMSE, $\text{Skill}_{\text{MAE}}$, and $\text{ExposureIndex}$ in $\mu\text{g}\cdot\text{h/m}^3$), `PG` (Architecture diagram `①`–`⑧`), `PH` (8-tool allowlist & 2025 AQI rules), `PI` (Fail-closed Flowchart & numbered Algorithm 1/Algorithm 2 pseudocode), `PJ` (Concrete Scenarios `S1` Morning Run, `S2` Sensitive Group, `S3` Stale Data Fallback), `PK` (Key points contribution), `PL` (Link to simulation), and `PM` (Uncertainty-overlap abstention bound $|\hat{C}(W_1) - \hat{C}(W_2)| < \tau_{\text{err}}$)

### Requirement: Section IV Experiment Q–V Structure and Empirical Honesty Guardrail
Section `IV. Experiment` SHALL follow the `Q` through `V` progression of the 2020 A–Z SOP (`Q` Quality and Quantity Metrics, `R` Related Methods to Compare, `S` Simulation Setup, `T` Tuning & QC Parameters, `U` Useful Phase W1 Empirical Results, and `V` Verify Effectiveness & Scientific Honesty Boundary).

#### Scenario: Verifying empirical W1 data and scientific honesty in Section IV
- **WHEN** Section `IV. Experiment` is checked against `docs/w1-data-integration.md`
- **THEN** it presents `Q` (Track A MAE/RMSE/Skill/regret & Track B tool/citation/rule/degradation/latency metrics), `R` (Persistence & 24h Seasonal Naive vs. Ridge/RF/XGBoost; Rule-Only vs. Agent+ML+Rules), `S` (6 Taichung stations, 70/15/15 split, rolling-origin, 30 Track B cases `B1`–`B6`), `T` (`dedup_identical`, `MAX_VALID_PM25_UG_M3 = 1000.0`, `reconstructed_from_observed_at`), `U` (Table III live snapshot and Table IV 123,055-hour inventory with exact SHA256 prefixes), and `V` (Table V dual-track matrix with explicit scientific honesty that W2–W6 ML/Agent scores are not pre-claimed)

### Requirement: Section V Conclusion W–Z Structure
Section `V. Conclusion` SHALL follow the `W` through `Z` progression of the 2020 A–Z SOP (`W` What Proposed recap, `X` eXcel scenario and methodological strengths, `Y` Yields from Phase W1 empirical audit and dual-track framework, and `Z` Zen scope limitations and Phases W2–W6 future work).

#### Scenario: Auditing Conclusion against W–Z SOP
- **WHEN** Section `V. Conclusion` is reviewed
- **THEN** it systematically covers `W` (motivation and AirGuard AI recap), `X` (station-scale dual-track and constrained ReAct advantages), `Y` (123,055 verified Taichung hourly observations, 95.49%–97.90% coverage, and cryptographic SHA256 reproducibility), and `Z` (exclusion of street-level routing/inhaled dose/medical diagnosis and roadmap for W2–W6 backtesting, P1 SHAP, and web deployment)
