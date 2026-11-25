# 06-reference Specification

## Purpose

Defines the IEEE conference reference formatting and citation integrity requirements for `ICEIB paper/06-Reference.tex` and the root driver `ICEIB paper/main.tex`.

## Requirements

### Requirement: IEEE Numeric Bibliography and Root Modular Compilation
The file `06-Reference.tex` SHALL provide consecutive IEEE-formatted `thebibliography` entries (`[1]`–`[24]`) resolving every `\cite{...}` key across `01-Introduction.tex` through `05-Conclusion.tex`, and `main.tex` SHALL assemble `00-Abstract` through `06-Reference` via `\input` with zero LaTeX errors.

#### Scenario: Verifying modular compilation and citation resolution on Overleaf
- **WHEN** `main.tex` and `00-Abstract.tex` through `06-Reference.tex` are compiled via `pdflatex` on Overleaf (`6b064a46a654dfea12d0fd00`)
- **THEN** all 24 references (`[1]`–`[24]`) resolve with zero undefined citations and `compile` reports `built_cleanly: true` and `error_count: 0`
