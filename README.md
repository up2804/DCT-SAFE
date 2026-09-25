# DCT-SAFE Reproducibility Package

**Title:** DCT-SAFE: A Reproducible Digital Cyber Twin for Safe Adaptive Intrusion Detection Under Concept Drift and Unreliable Feedback

## Purpose

This repository contains the completed experimental outputs, figures, configuration information, and manuscript associated with the DCT-SAFE study.

The study evaluates adaptive intrusion detection under:
- controlled concept drift,
- delayed feedback,
- contaminated feedback,
- persistence verification,
- cooldown control.

The central methodological principle is:

> Detect Drift ≠ Accept Feedback ≠ Update Model.

## Main completed evidence

1. Controlled synthetic Digital Cyber Twin experiments.
2. 120 paired operational runs.
3. 180-run-per-policy ablation.
4. CIC-IDS2017 external family-level validation with 20 runs.
5. Bootstrap confidence intervals and Wilcoxon paired testing.
6. Operational adaptation-frequency and false-adaptation analysis.

## Main result

Persistence+Cooldown retained approximately 89.85% of the drift-only Attack-F1 gain while reducing adaptation events by 50.82% and reducing false adaptations from 0.2 to zero per run.

## Repository structure

- `data/synthetic/` — completed synthetic run-level results
- `data/cicids_family/` — CIC-IDS2017 family-level results
- `analysis/` — Excel analysis packages
- `figures/` — publication figures
- `config/` — experimental configuration
- `manuscript/` — current manuscript
- `src/` — reserved for final executable source code

## Dataset note

The raw CIC-IDS2017 dataset is not redistributed in this repository. Users should obtain it from the Canadian Institute for Cybersecurity and follow the dataset's terms.

## Important interpretation notes

The synthetic cyber twin is a controlled simulation and is not claimed to reproduce a specific operational network.

The CIC-IDS2017 family experiment is external validation, but its temporal attack composition means that learning previously unseen attack families and concept-drift adaptation cannot be perfectly separated.

Incomplete Random Forest experiments are deliberately excluded from quantitative manuscript claims.

## Reproducibility

The final public release should include:
- executable source code,
- exact preprocessing,
- configuration files,
- fixed seeds,
- requirements/environment file,
- exact execution commands,
- raw run-level outputs,
- generated figures.

## Suggested citation

Singh, U. K. (2026). DCT-SAFE: A Reproducible Digital Cyber Twin for Safe Adaptive Intrusion Detection Under Concept Drift and Unreliable Feedback. Reproducibility package, version 1.0. Zenodo. DOI: to be assigned after publication.

## License

Recommended for code: MIT License.
Recommended for result data/documentation: CC BY 4.0, subject to journal/data-source restrictions.
