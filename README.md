# Replication: Landowner Preferences for Incentive Programs in North Carolina

## 1. Paper Replicated

Deviney, Courtney B., Rajan Parajuli, Frederick W. Cubbage, Erin O. Sills, and Robert E. Bardon. 2026. "Understanding Landowner Preferences for Traditional and Nature-Based Solutions Incentive Programs in North Carolina, USA." *PLOS ONE* 21 (4): e0347042.

https://doi.org/10.1371/journal.pone.0347042

## 2. Data Source

The replication uses `decoded_data.xls`, an Excel dataset containing information on North Carolina forest and farm landowners.

The published study provides its empirical dataset in the supporting information associated with the journal article.

The working dataset was obtained from the team's replication project.

**Original dataset:** https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0347042

## 3. How to Run the Replication

The analysis uses R. After installing R, open Terminal and run:

```bash
git clone https://github.com/LeopoldKronecker/econ5560-replication-pradhan.git
cd econ5560-replication-pradhan
Rscript run_all.R > logs/run_log.txt 2>&1
```

The master script checks for required packages, installs missing packages from CRAN, loads the dataset, runs the analysis, and saves the resulting tables and figures in `outputs/`.

The execution log is saved as `logs/run_log.txt` and includes R session information.

The script should be executed from the repository's root directory.

## 4. File Descriptions

- `run_all.R` — Master R script executing the replication analysis.
- `decoded_data.xls` — Dataset used for the replication.
- `combined_model_and_replication_report.qmd` — Quarto source document containing the team's replication report.
- `outputs/figure_landowner_distribution.png` — Visualization of forest and farm landowners by region.
- `outputs/table_sample_size_comparison.csv` — Sample-size comparison.
- `outputs/table1_variable_checklist.csv` — Checklist of variables used in the replication.
- `outputs/table2_summary_comparison.csv` — Summary statistics comparison.
- `outputs/table4_model_odds_ratios.csv` — Model odds-ratio results.
- `logs/run_log.txt` — Execution log, including package information and session details.
- `README.md` — Repository documentation and reproduction instructions.
- `.gitignore` — Excludes temporary and machine-specific files from version control.

## 5. Software and Packages

The replication was successfully executed on November 10, 2026, using R version 4.6.1 on macOS.

Required R packages:

| Package | Version |
|---|---|
| readxl | 1.6.0 |
| dplyr | 1.2.1 |
| tidyr | 1.3.2 |
| tibble | 3.3.1 |
| knitr | 1.52 |
| kableExtra | 1.4.1 |
| mvtnorm | 1.4-2 |
| ggplot2 | 4.0.3 |
| sandwich | 3.1-3 |
| lmtest | 0.9-40 |

These versions are taken from the successful execution log.

Quarto was not installed during the successful R pipeline execution. Rendering the separate `.qmd` report has not been verified.

## 6. Execution Time

The complete replication pipeline ran from 11:15:07 to 11:16:46 on November 10, 2026.

**Total execution time: approximately 1 minute and 39 seconds.**

Runtime may vary depending on hardware and package installation requirements.

## 7. Replication Results and Limitations

The master script was successfully executed from a fresh clone of this repository.

The run completed with exit code 0, generated five output files, and recorded the software environment through `sessionInfo()`.

No error messages were found using a search for "error" or "execution halted" in the execution log.

A successful execution does not necessarily demonstrate that every published result has been reproduced exactly. Agreement between the generated tables and figures and the original article requires separate verification.

The Quarto report has not been rendered independently.

[Add any verified differences between the published study and the replication results.]

## 8. Use of AI

ChatGPT was used to assist with Git commands, repository setup, understanding the fresh-clone verification procedure, and drafting replication documentation. The replication script originated from the team's existing project.
