# TiO0.5N0.5 FEFF/XAS Example

This directory documents an early MORPH demonstration based on a 12-atom titanium oxynitride cluster.

## Target absorption edges

- O K
- N K
- Ti K
- Ti L

## Recommended per-edge record

For each edge, preserve:

```text
edge_name/
├── feff.inp
├── xmu.dat
├── chi.dat
├── paths.dat
├── feffNNNN.dat
├── plots/
└── analysis/
```

The exact set of FEFF output files depends on the calculation and FEFF version.

## Analysis sequence

1. Confirm the absorber and FEFF input.
2. Inspect `xmu.dat` headers and identify every column before plotting.
3. Plot the physically defined absorption/background quantities.
4. Use `chi.dat` for χ(k) when available.
5. Apply a documented k-range, k-weight, and window before Fourier transformation.
6. Plot |χ(R)| over a stated R-range.
7. Compare R-space features with calculated scattering paths.
8. Do not identify a raw Fourier peak as a bond length without considering phase shifts.
9. Export figures, processed data, and a short analysis record.

## Structural interpretation

For Ti-centered K-edge EXAFS, Ti-O/Ti-N first-shell and Ti-Ti higher-shell paths may be physically relevant depending on the structural model. For O- or N-centered soft-edge calculations, shell labels must be assigned from the actual absorber-centered scattering geometry rather than transferred automatically from Ti-centered intuition.

This example directory is documentation only until validated input/output datasets and analysis scripts are added.
