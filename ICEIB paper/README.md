# ICEIB IEEE Conference Paper — AirGuard AI

- **Title**: *AirGuard AI: An Evidence-Grounded Domain AI Agent for Station-Scale Short-Term $\text{PM}_{2.5}$ Forecasting and Conservative Outdoor Activity Decision Support*
- **Authors**: Ming-Hsien Tsai (`7115056013`), Hung-Yang Lin (`7115056179`), and Ping-Kun Hsu (`8114056002`)
- **Target Conference**: IEEE International Conference on Electronic Communications, Internet of Things and Big Data (ICEIB, `www.iceib.asia`)
- **Overleaf Project**: [`AIoT_DA_DIC4` (`6b064a46a654dfea12d0fd00`)](https://www.overleaf.com/project/6b064a46a654dfea12d0fd00)

## Manuscript Files

| File | Format & Purpose |
|---|---|
| [`main.tex`](main.tex) | Compilable `IEEEtran` (`\documentclass[conference,a4paper]{IEEEtran}`) LaTeX source synchronized with Overleaf (`pdflatex`, 0 errors, 0 warnings) |
| [`main.txt`](main.txt) | Complete IEEE two-column conference manuscript in plain text for direct review or MS Word template insertion |

## 2020 A–Z SOP Section Mapping (`myRef/A2Z outline example.pdf`)

| Paper Section | 2020 A–Z SOP Building Blocks | Manuscript Implementation |
|---|---|---|
| **Abstract** | `A` Attention, `B` But, `C` Cure, `D` Development, `E` Experiments, `F` Findings | Single-paragraph abstract covering WHO (2019: 4.2M deaths) & MOENV (2019–2025 $\text{PM}_{2.5}$ $16.2 \rightarrow 12.8\,\mu\text{g/m}^3$), status-to-action & LLM/leakage challenges, AirGuard AI architecture, Phase W1 6-station Taichung audit (123,055 valid hours), and dual-track evaluation protocol |
| **I. Introduction** | `G` General, `H` However, `I` In Literature, `J` Judgement (SWOT), `K` Keypoint, `L` Organization | Subsections `I-A` (`G`), `I-B` (`H`), `I-C` (`I, J` SWOT critique), and `I-D` (`K` 4 contributions, `L` paper roadmap) |
| **II. Related Work** | `M` Methods (50% AI + 50% Domain), `N` New Proposed (Deep Research Q1–Q3 & Research Gap), `O` Organize (SWOT Table) | Subsections `II-A` (`M`), `II-B` (`N, O`), and **Table I** comparing representative AI and environmental exposure literature |
| **III. Proposed Design** | `PA` Aim, `PB` Background, `PC` Cure/Cause, `PD` Design Shift, `PE` Elements (`①`–`⑧`), `PF` Formulation, `PG` Graph, `PH` How, `PI` Flowchart & Pseudocode, `PJ` Examples (`S1`–`S3`), `PK` Key Contribution, `PL` Simulation Link, `PM` Math Bounds | Subsections `III-A` (`PA`–`PD`, **Table II** MOENV datasets), `III-B` (`PE, PG, PH`, **Fig. 1** Architecture `①`–`⑧` & Fail-Closed Flowchart), `III-C` (`PF, PI, PM`, Eqs. 1–6 & **Algorithms 1–2**), and `III-D` (`PJ`–`PL`, **Table III** Scenarios `S1`–`S3`) |
| **IV. Experiment** | `Q` Metrics, `R` Related Methods, `S` Setup, `T` Tuning/QC, `U` Useful Results, `V` Verify Effectiveness | Subsections `IV-A` (`Q, R`), `IV-B` (`S, T`), and `IV-C` (`U, V`, **Table IV** Taichung 6-station snapshot, **Table V** 33-month 123,055-hour quality inventory with SHA256 prefixes, and **Table VI** Dual-Track 30-scenario matrix) |
| **V. Conclusion** | `W` What Proposed, `X` eXcel, `Y` Yields, `Z` Zen (Limitations & Future Work) | Subsections `V-A` (`W, X`) and `V-B` (`Y, Z`) |
| **References** | IEEE Numeric Citation Style | Consecutive bracketed references `[1]`–`[24]` |
