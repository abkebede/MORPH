# MORPH Reproducible Workflow

A MORPH analysis should preserve the chain from source data to scientific conclusion.

## 1. Define the scientific question

State the observable, physical hypothesis, model, expected parameter range, and intended validation test before processing the data.

## 2. Preserve raw inputs

Do not overwrite raw experimental or simulation files. Record source, acquisition/simulation conditions, software version, units, and file-format definitions.

## 3. Verify file semantics

Before numerical analysis, inspect headers and documentation. Never infer the meaning of columns solely from their position. This is particularly important for simulation outputs such as FEFF `xmu.dat`.

## 4. Process with explicit parameters

Record normalization, background treatment, fit ranges, Fourier-transform ranges, window functions, k-weighting, interpolation, and any statistical preprocessing.

## 5. Separate calculation from interpretation

Produce calculated quantities first; then interpret them using physical models, scattering paths, calibration information, literature, or validated reference data.

## 6. Validate

Use one or more of the following as appropriate:

- reference calculations;
- experimental standards;
- known limiting behavior;
- alternative model formulations;
- held-out data;
- uncertainty or sensitivity analysis.

## 7. Export reproducible outputs

Each analysis should be able to produce:

- machine-readable processed data;
- publication-quality PNG/PDF figures;
- parameter tables;
- processing metadata;
- a concise methods record;
- software/environment information.

## 8. Archive

Tag stable repository versions. For published work, archive a release in a DOI-issuing repository when appropriate and cite the exact version used.
