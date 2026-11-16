# Hydraulic conductivity, infiltration flow, and CFD–DEM displacement data for aggregate-amended purple soil

This repository contains processed infiltration observations and numerical downslope particle-displacement histories supporting the manuscript **“Shear–scour CFD–DEM analysis of nonmonotonic erosion in aggregate-amended purple soil.”** The file and figure mapping follows the manuscript dated **16 November 2026**, prepared for submission to *Computers and Geotechnics*.

## Files and manuscript figures

| File | Current figure | Contents |
|---|---|---|
| `Fig10_Initial_conductivity_and_infiltration_flow.xlsx` | Fig. 10(a,b) | Initial-stage hydraulic conductivity and infiltration-flow observations for S0–S5 |
| `Fig10a_Initial_conductivity_plot_data.csv` | Fig. 10(a) | The 10 conductivity observations per mixture used in the box plots |
| `Fig10b_Infiltration_flow_plot_data.csv` | Fig. 10(b) | The 16 flow observations per mixture used in the box plots |
| `Fig12a_S0_y_displacement.xlsx` | Fig. 12(a) | S0 displacement histories at Mp1–Mp6 |
| `Fig12b_S1_y_displacement.xlsx` | Fig. 12(b) | S1 displacement histories at Mp1–Mp6 |
| `Fig12c_S2_y_displacement.xlsx` | Fig. 12(c) | S2 displacement histories at Mp1–Mp6 |
| `Fig12d_S3_y_displacement.xlsx` | Fig. 12(d) | S3 displacement histories at Mp1–Mp6 |
| `Fig12e_S4_y_displacement.xlsx` | Fig. 12(e) | S4 displacement histories at Mp1–Mp6 |
| `Fig12f_S5_y_displacement.xlsx` | Fig. 12(f) | S5 displacement histories at Mp1–Mp6 |

**Fig. 10. Initial-stage hydraulic conductivity and infiltration-flow distributions.**

**Fig. 12. Downslope particle displacement and final field erosion morphology.** The displacement workbooks contain the numerical curves. Field photographs are presented in the manuscript, not in these workbooks.

The earlier file `Figure 18-19.xlsx` maps to current Fig. 10, and the earlier `Fig. 21(a)`–`Fig. 21(f)` workbooks map to current Fig. 12(a–f). These old figure numbers identify historical filenames. The infiltration workbook is not runoff, sediment-concentration, or entropy-weighting data. The entropy-weighting procedure and indicator matrix are supplied separately in Supplementary Material S1 of the manuscript.

## Mixtures and monitoring points

S0, S1, S2, S3, S4, and S5 contain 0%, 10%, 20%, 30%, 40%, and 50% aggregates by volume, respectively.

| Point | Slope position | Depth below surface |
|---|---|---|
| Mp1 | Toe | Surface |
| Mp2 | Midslope | Surface |
| Mp3 | Crest | Surface |
| Mp4 | Crest | 0.20 m |
| Mp5 | Midslope | 0.20 m |
| Mp6 | Toe | 0.20 m |

The numerical coordinates are x across the slope, y downslope, and z vertical. Mp1–Mp6 identify monitoring positions, not experimental replicates.

## Variables and units

| Variable | Unit | Definition |
|---|---|---|
| Initial-stage hydraulic conductivity | m/d | Successive conductivity observations during the initial stage of the infiltration test |
| Infiltration flow | m³/d | Flow observations used to form the Fig. 10(b) distributions |
| Time | min | Recorded time supplied with each displacement history |
| Mp1–Mp6 y-displacement | m | Signed displacement in the downslope coordinate at each monitoring point |

The infiltration units follow the axes in Fig. 10 of the current manuscript; no numerical unit conversion has been applied. The original infiltration workbook did not state its units. The displacement source files explicitly state minutes and metres. Observation order in the infiltration files is a sequence index, not an inferred timestamp.

## Data used in Fig. 10

The Excel workbook retains its two original data blocks and all 174 source values. The six mixture columns are B, D, F, H, J, and L.

- **Fig. 10(a):** rows 3–12, with 10 observations per mixture.
- **Fig. 10(b):** rows 20–35, corresponding to observations 4–19 of the 19 available flow records. Column A identifies the records used in the figure. The first three flow records, in rows 17–19, remain in the workbook but are not included in Fig. 10(b).

The 16-record flow means for S0–S5 are 10.228750, 11.539750, 13.741875, 15.1696875, 19.234750, and 24.864750 m³/d. These reproduce the rounded figure labels. Counts of 10 and 16 describe successive observations through time; they are not counts of independent repeated experiments.

The CSV files provide the corresponding plotting subsets in a rectangular format. `source_excel_row` refers to the row in the Excel workbook, and `observation_index` refers to the observation order within its source block. Their six scheme columns retain the original numerical values. Conductivity CSV values are in m/d; flow CSV values are in m³/d.

## Displacement records and missing values

| Mixture | Records with time | Recorded time range (min) |
|---|---:|---|
| S0 | 7769 | 0.00695–59.99305 |
| S1 | 8184 | 0.00672–59.99756 |
| S2 | 7803 | 0.00683–59.99658 |
| S3 | 7829 | 0.00702–59.99425 |
| S4 | 7563 | 0.00714–59.99683 |
| S5 | 7645 | 0.00724–59.99940 |

Each workbook uses the supplied time vector directly. Sampling intervals vary between mixtures. Negative displacements are retained, including small reversals in S1 and S3 and the negative Mp5 interval in S5.

- **S4:** rows 7565–8404 contain 840 additional records for Mp2–Mp6, but time and Mp1 are missing. These 4200 displacement values remain in their original cells. Use records with a valid time for a time-history plot; the untimed tail cannot be placed on a time axis from this file alone.
- **S5:** Mp4 and Mp5 end at 59.85813 min. Their values are missing at the last 18 recorded times, from 59.86598 to 59.99940 min. Other point histories continue.

Blank cells and `--` denote missing entries, not zero. Numerical text has been converted to numerical Excel cells without changing its numerical value. Source signs, record order, missing entries, and endpoints are preserved. No interpolation, resampling, smoothing, or absolute-value transformation has been applied.

## Scope and contact

This deposit provides the processed infiltration and y-displacement records listed above. It does not contain the complete CFD–DEM model, FISH scripts, raw velocity histories, or HHT source data.

Manuscript authors: Yun Tian, Yongbo Tie, Xueling Li, Yong Wu, and Sen Li.

Corresponding authors: Yun Tian (tianyun@stu.cdut.edu.cn) and Yongbo Tie (tyb2009@qq.com).
