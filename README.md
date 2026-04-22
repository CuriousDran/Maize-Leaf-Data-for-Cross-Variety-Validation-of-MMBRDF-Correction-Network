# Maize-Leaf-Data-for-Cross-Variety-Validation-of-MMBRDF-Correction-Network
This space contains the data associated with published research with the same title as this repository. It contains maize leaf samples' MMBRDF model parameter data and the associated modelling, simulation, and analysis presented within the paper. 







## Introduction:
  Presenting curated maize MMBRDF model parameter data for three sampled varieties (B73, MO17, and Pioneer Hybrid). ​ A total of 25 samples were collected for each variety with the top five leaves of each of five plant samples are presented for all three varieties. ​ (i.e. B73 Plant 1-5 Leaf 1-5). ​ All samples were grown outdoors at Central Crops Research Station (CCRS) in Clayton, NC in the summer of 2024 ​
Publication in progress: "Cross-Variety Validation of a Polarimetric Glare Correction Algorithm for Maize" ​
Resources


##### BRDF_Sensitivity_Analysis_Code.zip: 
Contains Matlab scripts and functions used for sensitivity analysis. ​ Includes:

 - sensitivityAnalysis2025.m: the primary script for all data curation and analysis ​
 - BRDFProg.cpp: C++ script to run simulations on MMBRDF leaf models ​
 - sensitivity_analysis.sh: bash script to loop through and simulate each parameter simultaneously using BRDFProg.cpp ​


##### sensitivityAnalysisData_2025.zip: 
contains curated data for SCATMECH parameter sensitivity analysis. ​ 
Includes:
 - simulatedData: pre-curated dataset from sensitivity analysis with Monte Carlo simulations with C++ code (BRDFProg.cpp) ​
 - simulationStatisticalResults_2025.mat: simulation data statistics (RMSE) presented with binned values by scattering angle (scata) 
                                          and incidence angle (thetai) along with data labels ​


##### MMBRDF_ComparisonByVariety_Matlab_2025.zip: 
contains scripts and functions used in Matlab to perform statistical comparison of MMBRDF leaf data by variety. ​ 
Includes: 
 - correction_network_2023.mat: the same correction network developed and used in Plant Phenomics (BRDF correction) publication ​
                                scripts and functions to load, curate, evaluate CN, and present results ​


##### leafParameterSimData_CNvalidation_2025.zip: 
  contains curated MMBRDF leaf sample data after model-fitting and validation of previously developed correction network (CN). Simulated angle geometries are included and are the same set of values for each variety. ​     
                                             ​ 
Included Matlab tables are:
 - B73_parameterTable: contains all SCATMECH model parameter values for B73 specified by plant number (P#) and leaf number (L#) used for simulations. ​
 - MO17_parameterTable: contains all SCATMECH model parameter values for MO17 specified by plant number (P#) and leaf number (L#) used for simulations. ​
 - PH_parameterTable: contains all SCATMECH model parameter values for Pioneer Hybrid (PH) specified by plant number (P#) and leaf number (L#) used for simulations. ​
 - b73CNtable: containing corrected and uncorrected GNDVI calculated using data acquired from simulations along with angle geometries for each instance (thetai, thetas, phis) ​
 - mo17CNtable: containing corrected and uncorrected GNDVI calculated using data acquired from simulations along with angle geometries for each instance (thetai, thetas, phis) ​
 - phCNtable: containing corrected and uncorrected GNDVI calculated using data acquired from simulations along with angle geometries for each instance (thetai, thetas, phis) ​
