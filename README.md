# PhD Confirmation Milestone Report

This repository contains the working LaTeX source for the confirmation report
**Understanding and Exploiting Spatial Representation Transitions in Deep
Vision Models**. The report develops a representation-centred explainability
programme across three connected stages:

1. dataset-wide, layer-specific PCA-RGB analysis of CNN representations;
2. Adaptive K-DGRP for class-agnostic, gradient-free localization; and
3. J1 geometry distillation as an application of the observed transitions.

The immediate project stage is to complete the Adaptive K-DGRP and J1 papers;
the later transformer stage begins with a broad literature review and pilot,
then concentrates on the most informative architecture and explanatory object.

Orange evidence boxes mark figures, reruns, semantic analyses, or statistical
checks that still need to be inserted. They are intentionally explicit so that
unfinished evidence cannot be mistaken for a completed result.

## Compile in VS Code

1. Open this `milestone` folder in VS Code.
2. Open `main.tex`.
3. Save the file or run **LaTeX Workshop: Build LaTeX project**.
4. Open `build/main.pdf` using **LaTeX Workshop: View LaTeX PDF**.

The included settings use `latexmk`, which automatically runs BibTeX and the
required additional LaTeX passes.

## Compile in a terminal

Compile the manuscript (the programme diagram and Gantt chart are generated
directly from TikZ source):

```bash
latexmk -pdf -outdir=build main.tex
```

## Structure

- `main.tex`: paper entry point and packages
- `sections/01_introduction.tex`: motivation, questions, objectives, and scope
- `sections/02_related_work.tex`: broad critical review of attribution,
  perturbation, concept/prototype explanation, CAM, representation analysis,
  neural collapse, knowledge distillation, and transformer explanation
- `sections/03_method.tex`: research design and PCA-RGB methodology
- `sections/04_experiments.tex`: current PCA-RGB observations and controls
- `sections/05_results.tex`: Adaptive K-DGRP method and completed evidence
- `sections/06_conclusion.tex`: verified J1 objective and ImageNet-100 benchmark
- `sections/07_research_plan.tex`: claim--evidence map and staged two-year plan
- `sections/08_final_conclusion.tex`: overall conclusion
- `figures/`: editable TikZ source for the research programme and Gantt chart
- `references.bib`: BibTeX references
- `.vscode/settings.json`: LaTeX Workshop configuration

## Evidence status

The benchmark values supplied for J1, ReviewKD-120, H9, and the external
feature-distillation baselines are included exactly as provided. The report
describes single-seed comparisons as preliminary and treats J1 and
ReviewKD-120 as a practical tie under the current evidence. PCA-RGB semantic
examples, the Adaptive K-DGRP confirmatory rerun, and J1 representation analyses
remain labelled placeholders pending final artifacts.

The current draft cites 127 distinct works. Every bibliography entry is used in
the manuscript, including methodological sources for the principal-component,
robust-prototype, evaluation, hashing, and loss-balancing choices.

To use this at `C:\Users\jiazh\OneDrive - Monash University\Desktop\milestone`,
clone or pull the repository into that location, then open the folder itself in
VS Code.
