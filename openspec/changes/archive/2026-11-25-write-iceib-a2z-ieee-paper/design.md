# Design

## Context

The AirGuard AI manuscript (`ICEIB paper/main.tex` and `ICEIB paper/main.txt`) targets the IEEE International Conference on Electronic Communications, Internet of Things and Big Data (ICEIB, `www.iceib.asia`) and is synchronized to Overleaf project `AIoT_DA_DIC4` (`6b064a46a654dfea12d0fd00`). In addition to standard IEEE two-column formatting, the manuscript must transparently embody the instructor's **2020 A–Z SOP** (`myRef/A2Z outline example.pdf`) and the seven compliance dimensions in `myRef/AirGuard AI 專題規範落實度資訊圖表.png`. See `proposal.md` for full motivation and scope.

## Goals / Non-Goals

**Goals:**
- Structure the manuscript into the exact section hierarchy requested by the author: `Abstract`, `I. Introduction`, `II. Related Work`, `III. Proposed Design`, `IV. Experiment`, `V. Conclusion`, and `References`.
- Explicitly align every paragraph and subsection with the 2020 A–Z SOP building blocks (`A`–`F` in Abstract, `G`–`L` in Introduction, `M`–`O` in Related Work, `PA`–`PM` in Proposed Design, `Q`–`V` in Experiment, and `W`–`Z` in Conclusion).
- Keep `ICEIB paper/main.tex` (compilable `IEEEtran` LaTeX), `ICEIB paper/main.txt` (plain-text IEEE manuscript), the Overleaf project (`6b064a46a654dfea12d0fd00`), and the GitHub repository (`AIoT_DA_1125`) synchronized.

**Non-Goals:**
- Fabricating uncompleted Phase W2–W6 machine learning test metrics (`MAE`, `RMSE`, `Skill Score`) or agent benchmark pass rates.
- Claiming street-level low-pollution route navigation, personal inhaled microgram dose, or clinical medical diagnosis.

## Decisions

1. **Exact Section Naming & A-to-Z Sub-block Mapping**:
   - *Decision*: Use exact top-level Roman numeral headings matching the user's specification (`I. Introduction`, `II. Related Work`, `III. Proposed Design`, `IV. Experiment`, `V. Conclusion`) while organizing subsections and paragraphs strictly around the 2020 A–Z SOP (`A`–`F`, `G`–`L`, `M`–`O`, `PA`–`PM`, `Q`–`V`, `W`–`Z`).
   - *Rationale*: Directly satisfies both the IEEE ICEIB two-column style and the course's A2Z outline SOP grading rubric without awkward non-IEEE section headers.
   - *Alternatives considered*: Embedding literal `[A]`, `[B]`, `[PA]` tags in visible section titles versus weaving them naturally into IEEE subsections and topic sentences. We weave them cleanly into the IEEE subsections (and document the exact A–Z mapping in the manuscript and OpenSpec spec) so the compiled PDF reads as a polished IEEE Xplore publication while fulfilling every A–Z checkpoint.

2. **Inclusion of Concrete Scenarios (`PJ`: S1–S3) and SWOT Judgement (`J`, `O`)**:
   - *Decision*: Explicitly incorporate the three user application scenarios from the infographic (`S1` 40-minute morning jogging in Taichung, `S2` sensitive population outdoor activity under Moderate/Orange AQI, and `S3` stale data / API failure safe degradation) in Section `III. Proposed Design` (`PJ`), and explicit SWOT/Judgement critiques in Section `I` (`J`) and Section `II` (`O`, Table I).
   - *Rationale*: `myRef/A2Z outline example.pdf` and `myRef/AirGuard AI 專題規範落實度資訊圖表.png` highlight `J` (Judgement/SWOT), `O` (4x5 / Article Summary Table), and `PJ` (Jump to an example: S1–S3) as essential checkpoints.

3. **Dual-File & Live Overleaf Synchronization Pipeline**:
   - *Decision*: Maintain `ICEIB paper/main.tex` as the authoritative `IEEEtran` source, mirror all structural updates to `ICEIB paper/main.txt`, and push directly to Overleaf (`6b064a46a654dfea12d0fd00`) via `@netique/overleaf-mcp` followed by automated `pdflatex` compilation verification (`error_count === 0`).
   - *Rationale*: Guarantees that local files, GitHub (`AIoT_DA_1125`), and the live Overleaf PDF never drift out of sync.

## Risks / Trade-offs

- **[Risk] Page length vs. A–Z completeness** $\rightarrow$ *Mitigation*: Use compact IEEE booktabs tables (`\toprule`, `\midrule`, `\bottomrule`) and concise mathematical notation so all `A`–`Z` (`PA`–`PM`) elements fit cleanly within 6–7 IEEE A4 pages without LaTeX overfull box errors.
- **[Risk] Overleaf session cookie expiration (~5 days)** $\rightarrow$ *Mitigation*: Store session cookie in `%APPDATA%\overleaf-mcp\cookie.json` and verify compilation via the MCP `compile` tool after every edit.
