# FARSIGHT — Artifact Repository

This repository hosts the supplementary artifacts for the FARSIGHT framework
(*Financial Agent Robustness and Security Investigation and Global Holistic Testing*),
a structured methodology for evaluating the robustness and security of financial LLM agents.

## Contents

- **`Codebook.md`** — The evidence-based codebook used to apply the FARSIGHT framework.
  It lists the nine evaluation metrics (R1–R4, S1, S2.1–S2.3, S3), their binary
  evidence indicators, and the deterministic scoring rules used to assign
  `● Fully Robust / Low Risk`, `◆ Partial`, or `○ Not Robust / High Risk` ratings.
  The content here mirrors the codebook in the paper appendix.

- **`reviewed_paper.pdf`** — A reference bundle of the 15 financial LLM agent
  papers reviewed under the FARSIGHT framework. We include this bundle so that
  reviewers can verify, for any agent we score in the paper, that the
  evidence indicators we cite (mechanisms, diagrams, experimental results)
  are visible in the source paper. This is the dataset that underlies
  Table I (agent summary) and the per-agent justifications in the appendix.

## Note on Anonymity

This is the **double-blind submission version** of the artifact. To preserve
anonymity, certain components have been intentionally withheld from this
public release:

- A subset of the **experimental attack implementations** (the executable
  proof-of-concept attacks used to illustrate S1 / S2 / S3 threat models)
  is **not included** in this snapshot, because the implementation files
  contain identifying configuration, environment, and authorship metadata.
- Any **internal tooling, evaluator notes, and infrastructure-specific
  scripts** that could reveal the affiliation of the authors have been
  similarly redacted.

These omissions do not affect the framework itself or the reproducibility
of the scoring procedure: the codebook in `Codebook.md` is fully
deterministic, and any evaluator can re-derive every rating in the paper
from the cited papers in `reviewed_paper.pdf`.

**If the reviewers require the withheld attack artifacts, we are happy to
provide them upon request through the conference's anonymous communication
channel.** A de-anonymized release of all materials will accompany the
camera-ready version of the paper.
