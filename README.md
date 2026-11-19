# Infiltration and downslope particle displacement in rock-fragment-amended purple soil

This dataset accompanies the study *Balancing Infiltration and Scour Resistance of Purple Soil on Sloping Farmland via Colluvial Rock Fragment Amendment*. It contains processed double-ring infiltration measurements and simulated downslope particle displacement time series for six purple-soil mixtures. The field site was a cultivated slope in Anyue County, Sichuan, China. The local sandstone–mudstone fragments were crushed to 1–2 mm and mixed into the cultivated layer.

## File guide

The seven Excel workbooks correspond to the manuscript panels listed below. The workbooks for Figure 8 contain the simulated curves; the accompanying field photographs are shown in the manuscript.

| Data file | Manuscript panel | Contents |
|---|---|---|
| `Fig6cd.xlsx` | 6c, 6d | Infiltration workbook with both measurement series for all six mixtures |
| `Fig8a_S0_y_displacement.xlsx` | 8a | Unamended control (S0), 0% fragments by volume |
| `Fig8b_S1_y_displacement.xlsx` | 8b | S1, 10% fragments by volume |
| `Fig8c_S2_y_displacement.xlsx` | 8c | S2, 20% fragments by volume |
| `Fig8d_S3_y_displacement.xlsx` | 8d | S3, 30% fragments by volume |
| `Fig8e_S4_y_displacement.xlsx` | 8e | S4, 40% fragments by volume |
| `Fig8f_S5_y_displacement.xlsx` | 8f | S5, 50% fragments by volume |

## Reading the infiltration files

The six mixture columns in the Excel workbook are B, D, F, H, J and L, in order from S0 to S5. Rows 3–12 contain the conductivity values for Figure 6c. Rows 17–35 contain 19 infiltration-flow observations per mixture. Figure 6d uses the final 16 observations (rows 20–35); the first three observations remain in the workbook. Across the two series, the workbook contains 174 measurement values. The counts of 10 and 16 refer to successive observations within a test, not independent replicates.

In `Fig6cd.xlsx`, the first data block lists initial-stage hydraulic conductivity in m/day (Figure 6c). The second block lists infiltration flow in m³/day (Figure 6d); column A indicates which observations were used in that panel. Infiltration flow is a volumetric rate into the soil, not runoff discharge at the plot outlet.

## Reading the displacement files

Each workbook corresponds to one mixture and contains time (minutes) and signed displacement (metres) at six simulated monitoring points. The global *y* axis runs downslope. Negative values are part of the recorded motion. The pairs below identify a surface point and a second point 0.20 m below it at the same slope position.

| Slope position | Surface point | Shallow point |
|---|---|---|
| Toe | Mp1 | Mp6 |
| Midslope | Mp2 | Mp5 |
| Crest | Mp3 | Mp4 |

Rows with valid time stamps number 7,769 (S0), 8,184 (S1), 7,803 (S2), 7,829 (S3), 7,563 (S4) and 7,645 (S5). Use the time column in each file; the mixtures do not share a single time vector. Blank cells and `--` indicate missing entries, not zero.

- **S4:** Rows 7565–8404 retain 840 additional records for Mp2–Mp6. Time and Mp1 are missing on those rows. Exclude this untimed tail from plots of displacement against time.
- **S5:** The last recorded values for Mp4 and Mp5 occur at 59.85813 min. Those two columns are missing at the final 18 time stamps (59.86598–59.99940 min); the other point histories continue.

The displacement files preserve the recorded signs and endpoints. The series have not been interpolated, resampled or smoothed.

## Contact

Yun Tian: tianyun@stu.cdut.edu.cn  
Yongbo Tie: tyb2009@qq.com
