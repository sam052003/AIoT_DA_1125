# Tasks

## 1. Abstract (A–F) and Section I Introduction (G–L) Alignment

- [x] 1.1 Refine the Title, Author Block (`Ming-Hsien Tsai`, `Hung-Yang Lin`, `Ping-Kun Hsu`), `Abstract`, and `Index Terms` in `ICEIB paper/main.tex` and `ICEIB paper/main.txt` to explicitly follow the 2020 A–Z SOP `A` (Motivation), `B` (But), `C` (Cure), `D` (Development), `E` (Experiments), and `F` (Findings/Expected Outcomes) flow, and verify all six segments are present without fabricated metrics.
- [x] 1.2 Structure Section `I. Introduction` in `ICEIB paper/main.tex` and `ICEIB paper/main.txt` around `G` (General Current Status), `H` (However / Challenges), `I` (In Literature taxonomy from old to new / simple to complex), `J` (Judgement / SWOT critique), `K` (Keypoint & 4 numbered contributions), and `L` (List the Organization of Sections II–V), and verify all `G`–`L` subsections/paragraphs are complete.

## 2. Section II Related Work (M–O) and Deep Research Integration

- [x] 2.1 Organize Section `II. Related Work` in `ICEIB paper/main.tex` and `ICEIB paper/main.txt` into `M` (Methods: 50% AI Technology + 50% Environmental Domain Know-How from simple to complex), `N` (New Proposed: Deep Research 5 Mindsets Q1, 3 Controversies Q2, 10 Deep Questions Q3, and `Existing Research -> Limitations -> Research Gap -> AirGuard AI`), and `O` (Organize: SWOT / Article Summary Table I), and verify Table I and all `M`–`O` blocks render cleanly.

## 3. Section III Proposed Design (PA–PM) and Three Technical Representations

- [x] 3.1 Update Section `III. Proposed Design` heading and subsections in `ICEIB paper/main.tex` and `ICEIB paper/main.txt` to cover `PA` (Aim), `PB` (MOENV Open Data Background & Table II), `PC` (Dual-Track Cure/Cause separating official AQI from predicted $\text{PM}_{2.5}$), `PD` (Design Paradigm Shift), `PE` (Modules `①`–`⑧` Elements), `PF` (Mathematical Formulations for Baselines, Metrics, and $\text{ExposureIndex}$), `PG` (System Architecture Graph `①`–`⑧`), and `PH` (ReAct 8-Tool Allowlist & Versioned 2025 AQI Rules), and verify all mathematical and architectural components match `DESIGN.md`.
- [x] 3.2 Ensure Section `III. Proposed Design` in `ICEIB paper/main.tex` and `ICEIB paper/main.txt` includes `PI` (Fail-Closed Quality-Check Flowchart and line-numbered Pseudocode for Algorithm 1 `TrainAndEvaluate` and Algorithm 2 `AirGuardAgent`), `PJ` (Concrete Walkthrough Examples: Scenarios `S1` Morning Jogging, `S2` Sensitive Population Protection, and `S3` Stale/Abnormal Data Fallback), `PK` (Key Points Contribution), `PL` (Transition to Simulation/Evaluation), and `PM` (Deterministic Verification & Uncertainty-Overlap Abstention Bounds $|\hat{C}(W_1) - \hat{C}(W_2)| < \tau_{\text{err}}$), and verify both algorithms and scenarios `S1`–`S3` are present.

## 4. Section IV Experiment (Q–V), Section V Conclusion (W–Z), and References

- [x] 4.1 Update Section `IV. Experiment` heading and subsections in `ICEIB paper/main.tex` and `ICEIB paper/main.txt` to follow `Q` (Quality and Quantity Metrics for Track A & Track B), `R` (Related Methods to Compare: Persistence/Seasonal Naive vs. Ridge/RF/XGBoost; Rule-Only vs. Agent+ML+Rules), `S` (Simulation Setup across the 6 Taichung MOENV stations & 30 Track B scenarios `B1`–`B6`), `T` (Tuning & QC Parameters: `dedup_identical`, `MAX_VALID_PM25_UG_M3 = 1000.0`, `reconstructed_from_observed_at`), `U` (Useful Results: Empirical Phase W1 Tables III & IV across 123,055 valid hourly observations with SHA256 prefixes), and `V` (Verify Effectiveness: Dual-Track Matrix Table V & Scientific Integrity Statement), and verify all figures match `docs/w1-data-integration.md`.
- [x] 4.2 Update Section `V. Conclusion` and `References` in `ICEIB paper/main.tex` and `ICEIB paper/main.txt` to follow `W` (What Proposed), `X` (eXcel), `Y` (Yields), and `Z` (Zen: Scope Limitations & W2–W6 Future Work) with consecutive IEEE references `[1]`–`[24]`, and verify every citation key resolves properly.

## 5. Synchronization and Overleaf Compilation Verification

- [x] 5.1 Mirror `ICEIB paper/main.tex`, `ICEIB paper/main.txt`, and `openspec/` between the workspace root (`C:\Users\sam98\Desktop\AIoT_1125`) and the Git repository (`C:\Users\sam98\Desktop\AIoT_1125\AIoT_DA_1111`), push the updated `main.tex` to Overleaf project `AIoT_DA_DIC4` (`6b064a46a654dfea12d0fd00`) via `@netique/overleaf-mcp`, and verify `compile` succeeds with `built_cleanly: true` and `error_count: 0`.
