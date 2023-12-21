# Predicting_Annual_Variability_Renewable_Energy

EAEE 4000 (ML for Environmental Engineering), Group 3: A project by Avikal Sagar and Neha Gosula at Columbia University that involves forecasting the total electricity demand load based on climatic conditions and geographical regions, and further predicting the generation of electricity by each fuel type (renewable/non-renewable) that would cater to the total demand. Flow of Python notebooks:

1. Merging SPP data: involves merging all the SPP Generation Mix datasets for the Southwest US from 2018 to 2022. Each of them was extracted from: https://marketplace.spp.org/file-browser-api/download/generation-mix-historical?path=%2FGenMix_2019.csv by replacing the year in the link
2. Averaging SPP data: involves performing data transformation from a 15-min interval on to an hourly basis while also: handling dates and time in the Pandas datetime format, removing duplicates, sorting in chornological order and some basic data cleaning processes
3. ERA 5: involves extraction of climate data on the basis of spatial coordinates for each state in the Southwest US. First the data is extracted as raster images, then converted into structural/numerical format before being appended all together
4. XGBoosted Random Forest & NN: involves building both forward (multi-input/single-output) and inverse (single-input/multi-output) models using Xg boosted Random Forests and Deep NNs respectively, along with an example of "mini-deployment" of the final model at the end
5. LSTM: part of future development plans to replace the forward model with LSTMs too. Ongoing process.

For data used and PDF reports, refer to the corresponding files.

For other questions: email Avikal Sagar (avikal.sagar@columbia.edu).
