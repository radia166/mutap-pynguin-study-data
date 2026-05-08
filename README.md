# mutap-pynguin-study-data
This repository contains supplementary appendices for the master's thesis:
Comparative Evaluation of Automated Python Unit Test Generation:
Pynguin vs. MuTAP Across Open-Source and Industrial Codebases
The appendices include raw experimental data, per-module comparisons, and test quality metrics collected across 26 subject modules (14 open-source, 12 industrial) evaluated over 10 repeated runs per tool.

**Repository Contents**

**Appendix 1: Module-Level Mutation Score Comparison**

File: [Appendix_1_Module_Level_Comparison.csv](CSV/Appendix_1_Module_Level_Comparison.csv)

Per-module mutation scores for both tools across all 25 evaluated modules (13 paired open-source, 12 paired industrial). Includes mean mutation score, run-to-run standard deviation, mean difference between tools, absolute difference, and winner classification (MuTAP / Pynguin / Comparable). Also includes cross-domain coefficient of variation values.


**Appendix 2: Overall Mutation Comparison - Open-Source**

File: [Appendix_2_Mutation_Comparison_OpenSource.csv](CSV/Appendix_2_Mutation_Comparison_OpenSource.csv)

Detailed mutation score statistics for 14 open-source modules. Includes mean, median, standard deviation, minimum, and maximum mutation scores across 10 runs for both Pynguin and MuTAP, along with the mean delta (percentage points) between tools per module.

**Appendix 3: Overall Mutation Comparison - Industrial**

File: [Appendix_3_Mutation_Comparison_Industrial.csv](CSV/Appendix_3_Mutation_Comparison_Industrial.csv) 

Equivalent statistics to Appendix 2 for 12 industrial modules. Mutation scores are reported per module with full run-level descriptive statistics for both tools.

**Appendix 4: Mutation Score vs. Coverage Comparison - Open-Source**

File: [Appendix_4_Mutation_vs_Coverage_OpenSource.csv](CSV/Appendix_4_Mutation_vs_Coverage_OpenSource.csv)

Per-module comparison of line coverage, branch coverage, and mutation score for both tools across open-source subjects. 
Reports mean, minimum, and maximum values across 10 runs. Used to analyse whether structural coverage predicts fault detection capability.

**Appendix 5: Overall Coverage - Industrial**

File: [Appendix_5_Coverage_Industrial.csv](CSV/Appendix_5_Coverage_Industrial.csv)

Mean test count, mean line coverage, and mean branch coverage per industrial module for both tools across 10 runs. 
Used to compare coverage efficiency between tools in the industrial domain.

**Appendix 6: Quality vs. Execution Time - Open-Source**

File: [Appendix_6_Quality_vs_Time_OpenSource.csv](CSV/Appendix_6_Quality_vs_Time_OpenSource.csv)

Mean test generation time (seconds) and mean mutation score per open-source module for both tools. 
Used to analyse the trade-off between computational cost and test quality in the open-source domain.

**Appendix 7: Quality vs. Execution Time - Industrial**

File: [Appendix_7_Quality_vs_Time_Industrial.csv](CSV/Appendix_7_Quality_vs_Time_Industrial.csv)

Equivalent to Appendix 6 for industrial modules. Mean generation time and mean mutation score per module for both tools.

**Appendix 8: Test Complexity Summary**

File: [Appendix_8_Test_Complexity_Summary.csv](CSV/Appendix_8_Test_Complexity_Summary.csv)

Per-module and aggregate test complexity metrics for generated test suites. 
Includes lines of code (LOC), number of functions, cyclomatic complexity (CC), maintainability index (MI), 
and Pylint score for both tools across all 26 modules. Reports the percentage of tests achieving Grade A complexity and maintainability ratings.

**Experimental Setup**

  Tools evaluated: Pynguin (search-based) and MuTAP (adapted for local Llama 3.1 8B via Ollama)
  
  Mutation testing: MutPy (cross-subject analysis), MutMut (initial validation)
  
  Runs per module: 10 repeated independent runs per tool
  
  Subject modules: 14 open-source, 12 industrial (anonymised)
  
  Metrics: Mutation score, line coverage, branch coverage, test count, generation time, test complexity

**Notes**

Industrial module names are anonymised in the thesis to satisfy the collaborating organisation's confidentiality requirements. Anonymised labels (sub1 through sub12) are used consistently across all industrial appendices.
All data were collected under controlled experimental conditions as described in Chapter 4 of the thesis.
