# Biostatistical-analysis-of-DOX-MJNPs-FLA

This repository contains the analysis code for biostatistical analysis of DOX-MJNPs-FLA

## Requirements

- Python 3.10.9
- Jupyter
- NumPy 1.26.4
- Pandas 2.2.0
- Matplotlib 3.8.3
- SciPy 1.11.4
- Statsmodels 0.14.1
- Lifelines 0.28.0

## Entering Data

The data has been stored in CSV files, and the procedure for entering them for each analysis is explained accordingly.

1. **Hemolysis Data:**
   - The hemolysis data for the DOX-MJNPs-FLA group is stored in a CSV file. This file contains a column named `CONCENTRATION(mg/ml)` to input different concentrations of nanoparticles. Additionally, there are three other columns named `HEMOLYSIS1(%)`, `HEMOLYSIS2(%)`, `HEMOLYSIS3(%)`, representing the hemolysis data obtained from three repetitions at each concentration. Similarly, the hemolysis data for the MJNPs-FLA group is stored in a separate CSV file.

2. **Liver Enzymes Data:**
   - The data for each liver enzyme is stored in two separate CSV files named `LIVER ENZYMES (ALT)` and `LIVER ENZYMES (AST)`. The `LIVER ENZYMES (ALT)` file contains a `TREATMENT` column indicating the types of treatments (DOX, DOX/MJNPs-FLA, MJNPs-FLA, CONTROL). It also has three columns named `ALT1`, `ALT2`, `ALT3`, representing the levels of these enzymes in the blood for three repetitions of the experiment in each group. The `LIVER ENZYMES (AST)` file follows a similar structure, with a `TREATMENT` column and `AST1`, `AST2`, `AST3` columns for the enzyme levels.

3. **MTT Data:**
   - The MTT data for the DOX, DOX-MJNPs-FLA, and MJNPs-FLA groups are entered into three separate CSV files named `MTT (DOX)`, `MTT (DOX-MJNPs-FLA)`, and `MTT (MJNPs-FLA)` respectively. Each file contains four general columns: `CONCENTRATION` for the used concentrations and three columns named `VIABILITY`, representing the cell viability for three repetitions of the experiment.

4. **RT-PCR Data:**
   - The RT-PCR analysis data for the BAX and BCL2 genes are stored in two separate CSV files named `RT-PCR (BAX)` and `RT-PCR (BCL_2)`. Both files have 4 columns where the first column named `TREATMENT` indicates the types of interventions (Control, MJNPs-FLA, DOX, HT, DOX/MJNPs-FLA, MJNPs-FLA+EMF, DOX/MJNPs-FLA+EMF, DOX/MJNPs-FLA+EMF+HT). The next three columns named `FOLD CHANGE1`, `FOLD CHANGE2`, and `FOLD CHANGE3` represent the results from three repetitions.

5. **Survival Data:**
   - Survival data for analyzing the average survival and plotting the Kaplan-Meier curve is stored in a CSV file named `SURVIVAL`. This file has 3 columns: `TREATMENT` indicating the treatment groups (Control, DOX, MJNPs-FLA+EMF, DOX/MJNPS-FLA, MJNPs-FLA, DOX/MJNPS-FLA+EMF+HT, DOX/MJNPS-FLA+EMF, HT), `TIME` representing the time of sample death after each treatment in days, and `EVENT` showing with either 0 or 1 where 0 means the sample is alive and 1 means the sample is dead.

6. **Thermometry and CEM43 Data:**
   - Thermometry data for the control and MJNPs-FLA groups are stored in two separate CSV files named `THERMOMETRY (CONTROL)` and `THERMOMETRY (MJNPs-FLA)` respectively. Each file contains two columns where the first column `TIME` represents different measurement times, and due to three repetitions of each time, each time is repeated three times consecutively in this column. The next column named `TEMP` indicates the measured temperature.
