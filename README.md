# Subdaily_BROOK90: Modification of the R version of Federer's BROOK90 model to simulate a sub-daily water balance

[![Github All Releases](https://img.shields.io/github/downloads/hydrovorobey/Subdaily_BROOK90/total.svg)]()

**Licence**  
Attribution-NonCommercial-NoDerivatives 4.0 International (CC BY-NC-ND 4.0)

**Main reference**  
https://doi.org/10.5194/egusphere-2025-2084

## Model features
- Sub-daily time step and output (tested with 30-min data; the temporal resolution can be reduced to up to 1 min)
- Closed mass and energy balance
- Implementation of latent and sensible heat flux estimation

## Model input
- The model requires daily and sub-daily input data in the correct format (see examples in the test datasets).

**Daily-scale variables**
- Solar radiation (MJ m⁻²)  
- Maximum and minimum air temperature (°C)  
- Actual vapour pressure (kPa)  
- Wind speed (m s⁻¹)  
- Precipitation (mm)

**Sub-daily variables**
- Precipitation (mm)  
- Air temperature (°C)  
- Solar radiation (MJ m⁻²)  
- Wind speed (m s⁻¹)  
- Actual vapour pressure (kPa)  
- Soil heat flux (MJ m⁻²)

## The model files contain
- The BROOK90 physical lumped water balance model with a focus on a detailed representation of vertical water and energy fluxes at a sub-daily scale within the atmosphere–plant–soil system at a single site
- Sample data from ICOS stations in Saxony, Germany:
  - **DE-Tha** – mature spruce forest  
  - **DE-Hzd** – young oak forest  
  - **DE-Gri** – grassland  
  - **DE-Kli** – cropland  

These datasets include site parameters and pre-processed sub-daily and daily forcing data.

## Technical remarks
- The model is executed from the *RUN_MODEL.R* file and does not require additional installations.
- The framework currently runs in the **Global Environment**, meaning that all internal and output variables are stored there.

## Publications
- Kronenberg, R., Vorobevskii, I., Luong, T. T., Spank, U., Kim, D., & Mauder, M. (2025, under review).  
  *An extension of the BROOK90 hydrological model for estimation of subdaily water and energy fluxes.*  
  EGUsphere.  
  https://doi.org/10.5194/egusphere-2025-2084

- Vorobevskii, I., Kronenberg, R., Grünwald, T., & Mauder, M. (2026, under review).  
  *Significance of the multivariate time series consistency in micro-meteorological data for climate impact modelling.*  
  https://dx.doi.org/10.2139/ssrn.5915985
