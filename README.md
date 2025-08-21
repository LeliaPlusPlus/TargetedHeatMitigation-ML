# Simulating Targeted Afforestation for Urban Heat Mitigation with ML
This repository houses the code for the paper *Targeted urban afforestation can reduce income-based heat disparities in U.S. cities*.

## Abstract
Previous assessments on optimizing urban heat mitigation strategies, critical for urban planning and public health, have generally focused on a handful of cities, rarely considered logistical constraints for implementing common strategies, or used methods that poorly resolve urban-scale processes. Here, we fuse several satellite-derived estimates with a non-parametric machine learning approach to capture non-linearities in estimating thermal anomalies across 493 U.S. cities, enabling us to perform large-scale, computationally-efficient, data-driven simulations of afforestation and albedo management strategies for urban heat mitigation, including strategies targeting lower income neighborhoods. We find that 449 (361) cities have negative (positive) associations between income and daytime ΔAT (Δtree). All mitigation strategies lower daytime ΔAT, while targeted afforestation with albedo management (and without) lowers the daytime ΔAT for low income groups from 0.56±0.94℃ to 0.22±0.92℃ (and 0.24±0.93℃) and reduces the income-based ΔAT gap from -0.50±0.94℃ to -0.15±0.91℃ (and -0.17±0.93℃). Our results demonstrate the importance of targeted heat mitigation in low income communities, who have less options to adapt to extreme heat, to reduce urban heat disparities.

## Data availability
The data (which includes features, targets, demographics, and simulations) is housed on Zenodo. The notebook 0-DataProcessing.ipynb aggregates and cleans the data. In 6a, we output simulations. 
- data.csv contains the features, targets, and demoograghics
- simulations.csv contains the simulations by census tract

**NOTE:** The file data.csv contains the observed baseline, while the file simulations.csv contains the predicted baseline.

## Running the code
1. Download the data from Zenodo and place it into the data folder.
2. Ensure all relevant packages are downloaded (see requirements.txt).
3. Run notebooks 1-6c.
   1. Notebooks 6a-6c require the models trained in notebook 5b.

