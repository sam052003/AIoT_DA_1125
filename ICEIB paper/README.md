# ICEIB IEEE Conference Paper — AirGuard AI (Modular 2020 A–Z SOP Edition)

- **Title**: *AirGuard AI: An Evidence-Grounded Domain AI Agent for Station-Scale Short-Term $\text{PM}_{2.5}$ Forecasting and Conservative Outdoor Activity Decision Support*
- **Authors**: Ming-Hsien Tsai (`7115056013`), Hung-Yang Lin (`7115056179`), and Ping-Kun Hsu (`8114056002`)
- **Target Conference**: IEEE International Conference on Electronic Communications, Internet of Things and Big Data (ICEIB, `www.iceib.asia`)
- **Overleaf Project**: [`AIoT_DA_DIC4` (`6b064a46a654dfea12d0fd00`)](https://www.overleaf.com/project/6b064a46a654dfea12d0fd00)

## Modular Manuscript Files (`00`–`06` + `main`)

| File | OpenSpec Capability | 2020 A–Z SOP Blocks | Description |
|---|---|---|---|
| [`main.tex`](main.tex) | [`06-reference`](../openspec/specs/06-reference/spec.md) | Root Driver | `IEEEtran` (`conference,a4paper`) master file that assembles `00-Abstract` through `06-Reference` via `\input{...}` |
| [`00-Abstract.tex`](00-Abstract.tex) | [`00-abstract`](../openspec/specs/00-abstract/spec.md) | `A`–`F` | Abstract (`A` Motivation, `B` But, `C` Cure, `D` Development, `E` Experiments, `F` Findings) & `IEEEkeywords` |
| [`01-Introduction.tex`](01-Introduction.tex) | [`01-introduction`](../openspec/specs/01-introduction/spec.md) | `G`–`L` | Section I: `G` General Status, `H` However, `I` In Literature, `J` Judgement (SWOT), `K` Keypoint (4 Contributions), `L` Organization |
| [`02-Related Work.tex`](02-Related%20Work.tex) | [`02-related-work`](../openspec/specs/02-related-work/spec.md) | `M`–`O` | Section II: `M` Methods (50% AI + 50% Domain), `N` Deep Research Q1–Q3 & Research Gap, `O` SWOT Comparison **Table I** |
| [`03-Proposed Design.tex`](03-Proposed%20Design.tex) | [`03-proposed-design`](../openspec/specs/03-proposed-design/spec.md) | `PA`–`PM` | Section III: **Table II** MOENV Datasets, **Fig. 1** Architecture `①`–`⑧` & Fail-Closed Flowchart, Eqs. (1)–(6), **Algorithms 1–2**, **Table III** Scenarios `S1`–`S3` |
| [`04-Experiment.tex`](04-Experiment.tex) | [`04-experiment`](../openspec/specs/04-experiment/spec.md) | `Q`–`V` | Section IV: Metrics (`Q`), Baselines (`R`), Setup (`S`), QC Tuning (`T`), Phase W1 Empirical **Tables IV–V** (`U`), and Dual-Track Matrix **Table VI** (`V`) |
| [`05-Conclusion.tex`](05-Conclusion.tex) | [`05-conclusion`](../openspec/specs/05-conclusion/spec.md) | `W`–`Z` | Section V: `W` What Proposed, `X` eXcel, `Y` Yields, `Z` Zen (Limitations & Future Work) + Acknowledgment |
| [`06-Reference.tex`](06-Reference.tex) | [`06-reference`](../openspec/specs/06-reference/spec.md) | IEEE Citations | Consecutive IEEE `thebibliography` references `[1]`–`[24]` |
| [`main.txt`](main.txt) | Full Plain-Text Mirror | `A`–`Z` (`PA`–`PM`) | Combined plain-text IEEE conference manuscript for text review or MS Word template insertion |
