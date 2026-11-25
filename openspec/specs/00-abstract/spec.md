# 00-abstract Specification

## Purpose

Defines the IEEE ICEIB formatting and 2020 A–Z SOP (`A`–`F`) requirements for `ICEIB paper/00-Abstract.tex` (included by `main.tex`), covering the Abstract and Index Terms of the AirGuard AI manuscript.

## Requirements

### Requirement: Abstract A–F Rhetorical Structure and Index Terms
The file `00-Abstract.tex` SHALL present a single coherent paragraph (150–250 words) following the six rhetorical elements of the 2020 A–Z SOP (`A` Motivation, `B` But, `C` Cure, `D` Development, `E` Experiments, and `F` Findings/Expected Outcomes) followed by `IEEEkeywords`, without fabricating unverified experimental results.

#### Scenario: Auditing 00-Abstract.tex against A–F SOP
- **WHEN** `00-Abstract.tex` is evaluated against `myRef/A2Z outline example.pdf`
- **THEN** it includes `A` (WHO 2019 4.2M deaths and MOENV 2019–2025 $\text{PM}_{2.5}$ trend $16.2 \rightarrow 12.8\,\mu\text{g/m}^3$), `B` (status-to-action gap, leakage risks, and LLM AQI/$\text{PM}_{2.5}$ conflation), `C` (AirGuard AI Domain AI Agent), `D` (4 MOENV datasets, 1/3/6h baselines vs. Ridge/RF/XGBoost, 2025 AQI rules, 8-tool ReAct agent, $\mu\text{g}\cdot\text{h/m}^3$ exposure index), `E` (Phase W1 6-station Taichung audit and Track A/B protocol), and `F` (station-scale scope boundary and expected outcomes)
