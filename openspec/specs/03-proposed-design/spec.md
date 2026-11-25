# 03-proposed-design Specification

## Purpose

Defines the IEEE ICEIB formatting, three required technical representations, and 2020 A–Z SOP (`PA`–`PM`) requirements for Section III (`ICEIB paper/03-Proposed Design.tex`).

## Requirements

### Requirement: Section III Proposed Design PA–PM Structure and Three Technical Representations
The file `03-Proposed Design.tex` SHALL follow the `PA` through `PM` progression of the 2020 A–Z SOP and MUST include all three required technical representations: the eight-module architecture (`①`–`⑧`), the fail-closed quality-check flowchart, and line-numbered pseudocode for Algorithm 1 and Algorithm 2.

#### Scenario: Verifying PA–PM elements and three technical representations in 03-Proposed Design.tex
- **WHEN** `03-Proposed Design.tex` is reviewed
- **THEN** it covers `PA` (Aim), `PB` (MOENV datasets Table II & data contracts), `PC` (Dual-track Official AQI vs. Predicted $\text{PM}_{2.5}$), `PD` (Design paradigm shift), `PE` (Modules `①`–`⑧`), `PF` (mathematical formulations for Persistence, Seasonal Naive, MAE, RMSE, $\text{Skill}_{\text{MAE}}$, and $\text{ExposureIndex}$ in $\mu\text{g}\cdot\text{h/m}^3$), `PG` (Architecture diagram `①`–`⑧`), `PH` (8-tool allowlist & 2025 AQI rules), `PI` (Fail-closed Flowchart & numbered Algorithm 1/Algorithm 2 pseudocode), `PJ` (Concrete Scenarios `S1` Morning Run, `S2` Sensitive Group, `S3` Stale Data Fallback), `PK` (Key points contribution), `PL` (Link to simulation), and `PM` (Uncertainty-overlap abstention bound $|\bar{C}(W_1) - \bar{C}(W_2)| < \tau_{\text{err}}$)
