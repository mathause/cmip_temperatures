# Mean temperature anomalies for CMIP5 and CMIP6

Document mean temperature anomalies for time periods in cmip5 and cmip6 data. Check the [global warming levels](https://github.com/mathause/cmip_warming_levels) repository for a list of the year when a certain global warming level is reached.

*Mathias Hauser*<sup>1</sup>

<sup>1</sup>Institute for Atmospheric and Climate Science, ETH Zurich, Zurich, Switzerland

## Disclaimer

This data archive is created and maintained in an voluntary effort by its creators. The data are provided without warranty of any kind. Please note that the ownership of all files in the archive remains with the original providers! That means you should still acknowledge the CMIP6 data providers. This work is published under a [CC BY-SA 4.0](http://creativecommons.org/licenses/by-sa/4.0/) license by the authors. If you use the this archive please cite TODO.

## Multi model mean

:warning: The multi model mean depends on the models that are in the ensemble. A ensemble of opportunity is used here: all available models are included. Only one simulation per model is included. For the individual models please see below.

### CMIP6

**Table 1**: Multi-model mean global-mean temperatures for selected time periods and shared socioeconomic pathways (SSPs). Number in brackets indicates number of models in the ensemble. The same information can be found in a csv file [cmip6_mmm_temperatures_one_ens_1850_1900.csv](cmip6_mmm_temperatures_one_ens_1850_1900.csv).

| period    |   SSP1-1.9 (14) |   SSP1-2.6 (41) |   SSP2-4.5 (42) |   SSP3-7.0 (35) |   SSP5-8.5 (44) |
|:----------|----------------:|----------------:|----------------:|----------------:|----------------:|
|           |            (°C) |            (°C) |            (°C) |            (°C) |            (°C) |
| 2021-2040 |            1.53 |            1.61 |            1.64 |            1.6  |            1.73 |
| 2041-2060 |            1.67 |            1.95 |            2.19 |            2.31 |            2.63 |
| 2081-2100 |            1.53 |            2.06 |            3.01 |            4.04 |            4.99 |
| 2016-2035 |            1.42 |            1.48 |            1.49 |            1.44 |            1.54 |
| 2046-2065 |            1.67 |            1.99 |            2.33 |            2.51 |            2.88 |
| 2011-2020 |            1.28 |            1.34 |            1.34 |            1.29 |            1.37 |
| 2021-2030 |            1.53 |            1.61 |            1.64 |            1.6  |            1.73 |
| 2031-2040 |            1.66 |            1.81 |            1.91 |            1.94 |            2.15 |
| 2041-2050 |            1.67 |            1.95 |            2.19 |            2.31 |            2.63 |
| 2051-2060 |            1.65 |            2.02 |            2.44 |            2.72 |            3.15 |
| 2061-2070 |            1.62 |            2.06 |            2.65 |            3.14 |            3.73 |
| 2071-2080 |            1.58 |            2.08 |            2.85 |            3.58 |            4.35 |
| 2081-2090 |            1.53 |            2.06 |            3.01 |            4.04 |            4.99 |
| 2091-2100 |            1.5  |            2.04 |            3.08 |            4.27 |            5.31 |

### CMIP5

**Table 2**: Multi-model mean global-mean temperatures for selected time periods and representative concentration pathways (RCPs). Number in brackets indicates number of models in the ensemble. The same information can be found in a csv file [cmip5_mmm_temperatures_one_ens_1850_1900.csv](cmip5_mmm_temperatures_one_ens_1850_1900.csv).

| period    |   RCP2.6 (21) |   RCP4.5 (30) |   RCP6.0 (14) |   RCP8.5 (32) |
|:----------|--------------:|--------------:|--------------:|--------------:|
|           |          (°C) |          (°C) |          (°C) |          (°C) |
| 2021-2040 |          1.53 |          1.56 |          1.46 |          1.71 |
| 2041-2060 |          1.72 |          2    |          1.86 |          2.49 |
| 2081-2100 |          1.69 |          2.49 |          2.83 |          4.36 |
| 2016-2035 |          1.44 |          1.44 |          1.36 |          1.54 |
| 2046-2065 |          1.72 |          2.09 |          1.95 |          2.71 |
| 2011-2020 |          1.36 |          1.32 |          1.27 |          1.39 |
| 2021-2030 |          1.53 |          1.56 |          1.46 |          1.71 |
| 2031-2040 |          1.66 |          1.79 |          1.66 |          2.07 |
| 2041-2050 |          1.72 |          2    |          1.86 |          2.49 |
| 2051-2060 |          1.73 |          2.17 |          2.06 |          2.95 |
| 2061-2070 |          1.72 |          2.31 |          2.31 |          3.42 |
| 2071-2080 |          1.7  |          2.42 |          2.6  |          3.89 |
| 2081-2090 |          1.69 |          2.49 |          2.83 |          4.36 |
| 2091-2100 |          1.68 |          2.51 |          2.92 |          4.61 |


## Individual models

Temperature anomalies for individual models can be found in separate folders for [cmip6](temperatures/cmip6/csv/) and [cmip5](temperatures/cmip5/csv/)

### Example
The data is available in csv files:
``` csv
model, ens, exp, postprocess, table, grid, varn, period, mean
CAMS-CSM1-0, r1i1p1f1, ssp119, global_mean, Amon, gn, tas, 2021-2040, 1.07
CNRM-ESM2-1, r1i1p1f2, ssp119, global_mean, Amon, gr, tas, 2021-2040, 1.32
CanESM5, r1i1p1f1, ssp119, global_mean, Amon, gn, tas, 2021-2040, 2.16
...
```

### Files

There are two files with [cmip6](temperatures/cmip6/csv/) data. One with one ensemble member per model and one with all ensemble members. For [cmip5](temperatures/cmip5/csv/) two additional files are provided. The reference period is 1850 to 1900, however, many cmip5 models only start after 1850 and are therefore excluded. These models are also included in the `*_no_bounds_check.yml` files.

## Data
 * Monthly temperature data (variable: `tas`, Table ID: `Lmon`) for `historical` and
   * `RCP2.6`, `RCP4.5`, `RCP6.0`, and `RCP8.5` (CMIP5)
   * `SSP1-1.9`, `SSP1-2.6`, `SSP2-4.5`, `SSP3-7.0`, and `SSP5-8.5` (CMIP6)
 * Grid-cell area for atmospheric grid variables (`areacella`)

## Method
To calculate the temperature anomalies the following method is used for every individual model:
 1. Calculate global mean temperature (weighted with the grid cell area (`areacella`) if available, else the `cos` of the latitude is used)
 2. Calculate annual mean (Note: all months are weighted equally)
 3. Concatenate historical data and projection (constrained to the historical/ future time period)
 4. Subtract the mean over 1850 to 1900 (inclusive)
 5. Calculate the mean over the indicated time period

## Code
The code will be published in https://github.com/IPCC-WG1 as soon as I have the right to create a repository.

## Changelog

The changelog of the repository can be found under [CHANGELOG.md](CHANGELOG.md).


## License

CMIP TEMPERATURES is licensed under a Creative Commons Attribution-ShareAlike 4.0 International License.

A copy of the license is availabe at [LICENSE](LICENSE). If not, see [CC BY-SA 4.0](http://creativecommons.org/licenses/by-sa/4.0/).

### CMIP5 Data License Statement

The underlying raw data are published under the license of CMIP5. Terms of use for CMIP5 are applied for the derived data presented here. They are provided at https://pcmdi.llnl.gov/mips/cmip5/terms-of-use.html. Data from some modelling centres are licensed for use in non-commercial research and for educational purposes, other for unrestricted use. Please refer to the [terms of use for the CMIP5 modeling groups](https://pcmdi.llnl.gov/mips/cmip5/docs/CMIP5_modeling_groups.pdf) for details.
The data should be cited by its DOI and according to the [citation recommendation of CMIP5](https://pcmdi.llnl.gov/mips/cmip5/citation.html).

### CMIP6 Data License Statement

The raw CMIP6 data are licensed under Creative Commons [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0), following the [CMIP6 Terms of Use](https://pcmdi.llnl.gov/CMIP6/TermsOfUse). Note that some models publish the data under a non-commercial license ([CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/)). The license for each particular model dataset can be obtained at the [ESGF CoG portal](https://esgf-node.llnl.gov/search/cmip6) as part of the data citation information.

## Acknowledgment

We thank Urs Beyerle for downloading and curating the CMIP5 and CMIP6 data at the Institute for Atmospheric and Climate Science, ETH Zurich, Zurich, Switzerland.

### CMIP5

We acknowledge the World Climate Research Programme's Working Group on Coupled Modelling, which is responsible for CMIP, and we thank the climate modeling groups (listed in [cmip5_models.md](cmip5_models.md)) for producing and making available their model output. For CMIP the U.S. Department of Energy's Program for Climate Model Diagnosis and Intercomparison provides coordinating support and led development of software infrastructure in partnership with the Global Organization for Earth System Science Portals.”

### CMIP6

We acknowledge the World Climate Research Programme, which, through its Working Group on Coupled Modelling, coordinated and promoted CMIP6. We thank the climate modeling groups for producing and making available their model output, the Earth System Grid Federation (ESGF) for archiving the data and providing access, and the multiple funding agencies who support CMIP6 and ESGF.
