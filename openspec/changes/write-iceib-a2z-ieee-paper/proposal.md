# Proposal

## Why

The AirGuard AI research paper for the IEEE International Conference on Electronic Communications, Internet of Things and Big Data (ICEIB, `www.iceib.asia`) must strictly conform to both standard IEEE two-column conference formatting and the instructor's **2020 A–Z SOP** (`myRef/A2Z outline example.pdf` and `myRef/AirGuard AI 專題規範落實度資訊圖表.png`). Establishing a formal OpenSpec specification for the manuscript's sections (`Abstract`, `I. Introduction`, `II. Related Work`, `III. Proposed Design`, `IV. Experiment`, `V. Conclusion`, and `References`) and A-to-Z rhetorical building blocks ensures every paragraph, figure, table, algorithm, and Overleaf build satisfies both the course rubric and IEEE ICEIB publication standards.

## What Changes

- Formalize the **ICEIB IEEE Conference Manuscript Specification** (`iceib-a2z-paper-structure`) governing the required sections (`Abstract`, `I. Introduction`, `II. Related Work`, `III. Proposed Design`, `IV. Experiment`, `V. Conclusion`, `References`), IEEE two-column A4 typography/layout, author ordering (`Ming-Hsien Tsai`, `Hung-Yang Lin`, `Ping-Kun Hsu`), and Overleaf synchronization.
- Map the complete **2020 A–Z SOP** rhetorical sequence across every section of the paper:
  - **Abstract (`A`–`F`)**: `A` Attention Getter Motivation, `B` But (Challenge), `C` Cure (Proposed Solution), `D` Development (Method), `E` Experiments, `F` Findings / Expected Outcomes.
  - **I. Introduction (`G`–`L`)**: `G` General Current Status, `H` However (Expanded Challenges), `I` In Literature (Taxonomy from Old to New / Simple to Complex), `J` Judgement (SWOT / Pros & Cons Critique), `K` Keypoint (Design Spirit, Novelty & Major Goals / Contributions Summary), `L` List the Organization.
  - **II. Related Work (`M`–`O`)**: `M` Methods (50% AI Technology + 50% Environmental Domain Know-how categorized from old to new, simple to complex), `N` New Proposed (Existing Research $\rightarrow$ Limitations $\rightarrow$ Research Gap $\rightarrow$ Our Project + Deep Research 5 Mindsets, 3 Controversies, and 10 Deep Questions), `O` Organize (Judgement/SWOT structured comparison table).
  - **III. Proposed Design (`PA`–`PM`)**: `PA` Aim/Statement, `PB` Background/Benefit (MOENV datasets), `PC` Cure/Cause (Dual-track official AQI vs. predicted $\text{PM}_{2.5}$), `PD` Design Paradigm Shift, `PE` Paper Elements (Modules ①–⑧), `PF` Formulation/Foundation ($\text{PM}_{2.5}$ horizons $h \in \{1,3,6\}$, baselines, $\text{ExposureIndex}$), `PG` Graph (System Architecture Diagram ①–⑧), `PH` How (ReAct + 8-Tool Allowlist + 2025 MOENV AQI Rules), `PI` Implementation/Interaction (Quality-Check Flowchart & numbered Pseudocode for Algorithm 1 `AirGuardAgent` and Algorithm 2 `TrainAndEvaluate`), `PJ` Jump to an Example (Scenarios S1 Morning Run, S2 Sensitive Group, S3 Stale/Abnormal Data Fallback), `PK` Key Points Contribution, `PL` Later How to Do Simulation, `PM` Mathematical/Deterministic Verification Bounds.
  - **IV. Experiment (`Q`–`V`)**: `Q` Quality and Quantity Metrics (Track A MAE/RMSE/Skill Score; Track B Tool Selection, Provenance, Rule Consistency, Safe Degradation, Latency), `R` Related Methods to Compare (Persistence, Seasonal Naive vs. Ridge, RF, XGBoost; Rule-Only vs. Agent+ML+Rules), `S` Simulation Setup (Taichung 6 MOENV stations, 70/15/15 chronological split, Rolling-origin, 30 test cases B1–B6), `T` Tuning Parameters & QC Thresholds, `U` Useful Results (Empirical Phase W1 6-station data audit & SHA256 reproducibility), `V` Verify Effectiveness & Scientific Honesty Boundary.
  - **V. Conclusion (`W`–`Z`)**: `W` What Proposed (Review of Motivation & Challenges), `X` eXcel (Target Scenario & Algorithmic Strengths), `Y` Yields (Empirical W1 Data Audit, Dual-Track Protocol & Deliverables), `Z` Zen (Scope Limitations & W2–W6 Future Work).
  - **References**: Sequential IEEE bracketed citations (`[1]`–`[24]`).

## Capabilities

### New Capabilities
- `iceib-a2z-paper-structure`: Full structural, rhetorical (2020 A–Z SOP), technical (8-module architecture, flowchart, dual pseudocode algorithms, W1 empirical data tables, dual-track evaluation), and IEEE ICEIB formatting specification for the AirGuard AI conference manuscript (`ICEIB paper/main.tex` and `ICEIB paper/main.txt`) and its Overleaf project (`6b064a46a654dfea12d0fd00`).

### Modified Capabilities
<!-- No existing capabilities in openspec/specs/ are being modified. -->

## Impact

- Manuscript files: `ICEIB paper/main.tex` and `ICEIB paper/main.txt` (both in `AIoT_DA_1111/ICEIB paper/` and workspace root `ICEIB paper/`).
- Overleaf project synchronization: Overleaf project `AIoT_DA_DIC4` (`6b064a46a654dfea12d0fd00`) via `@netique/overleaf-mcp`.
- Reference assets consumed: `myRef/A2Z outline example.pdf` and `myRef/AirGuard AI 專題規範落實度資訊圖表.png`.
