This **Readme** includes how to run the scripts in this repo and how to reproduce the results in a manuscript on thermal acclimation in ecosystem respiration. The code has been tested using R version 4.3.1 on the platform aarch64-apple-darwin20  

**Step 1**: run "Acclimation_strength_USIB2_example.Rmd". This shows how thermal acclimation strength at the Ameriflux site USIB2 was calculated. This script also generates three data files (US-IB2_gap_filled_data.csv, US-IB2_nongap_filled_data.csv, US-IB2_data_estimate_acclimation.RDS) that will be used in Step 3. The data files generated by all the 93 study sites are uploaded to the EDI (data link will be provided when the data submission is approved). This will take a few minutes to finish running.  

**Step 2**: run "Acclimation_driver_analysis.Rmd". This reproduces the results about the drivers of thermal acclimation using Random Forest. This will take about 10 minutes to finish running.  

**Step 3**: run "Acclimation_effect_on_future_respiration.Rmd". This script reproduces future respiration rates under different acclimation scenarios. Running this script needs the three data files generated by Step 1. On this GitHub, only the site USIB2 data was provided, so this script only calculate the future respriations at this site. To calculate future respiration for all the 93 study sites, users need to run this script with data files from other sites. These data are uploaded to the EDI (data link will be provided when the data submission is approved). When running this script with data from all 93 sites, the results should be the same as the file "acclimation_data_future_complete.csv". This will take a couple of minutes to finish running for one site.  
