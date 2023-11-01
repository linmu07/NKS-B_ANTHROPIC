# Progresses of ANTROPIC project 

# *(WP1: Hindcast simulation)*

## 1. Methodology

### 1.1. Main tasks of WP1:
 1. Validate NorESM by the observations of radiotracers and chemical tracers; 
 2. Investigate historical hydrodynamics with validated modeling results

### 1.2. Model setup 
* **NorESM:** Ocean-ice configuration
* **Time period:** 1945 - near present

### 1.3. Tracer Setup
#### 1.3.1. Radiotracers:
* **Reprocessing plants:** liquid discharges from two European nuclear reprocessing plants and Sellafield and La Hague
 1. **Tc-99, I-129 & Cs-137:** documented discharge data for Sellafield since 1952 and for La Hague since 1966 (HELCOM, OSPAR, and RADD databases)
 2. **U-236:** a) documented discharge data for La Hague since 1966 (HELCOM databases);b) reconstructed discharges data for Sellafield and La Hague since 1971 (Castrillejo et al., 2020)

* **Global fallout:** atmospheric depostion from nuclear weapon testing
 * **Cs-137 & U-236:** resolved spatiotemporal deposition pattern (UNSCEAR 2000)

#### 1.3.2. **Vitual traers:**
* **Water masses in AO:** constent concentrations in entering water
 * Pacific water: 
 * Atlantic water (via Fram Strait & Barent Sea)
 * Fresh water
* **Point sources:** constent discharges
 * Sellafield
 * La Hague
 * Fukushima

## 2. Results

### 2.1. Radiotracer transport

| RP-derived Tc-99 | RP-derived I-129 |
| --- | --- |
| <video style="width:100%" controls src="/Users/mulin/Research/03_simulation/03_study_case/02_NorESM_NAO_AO/03_data_analysis/01_data_visualisation/04_plot/hist_trc_surf_RPTc99_lite.mp4"/> | <video style="width:100%" controls src="/Users/mulin/Research/03_simulation/03_study_case/02_NorESM_NAO_AO/03_data_analysis/01_data_visualisation/04_plot/hist_trc_surf_RPI129_lite.mp4"/> |

| **RP-derived Cs-137** | **GF-derived Cs-137** |
| --- | --- |
| <video style="width:100%" controls src="/Users/mulin/Research/03_simulation/03_study_case/02_NorESM_NAO_AO/03_data_analysis/01_data_visualisation/04_plot/hist_trc_surf_RPCs137_lite.mp4"/> | <video style="width:100%" controls src="/Users/mulin/Research/03_simulation/03_study_case/02_NorESM_NAO_AO/03_data_analysis/01_data_visualisation/04_plot/hist_trc_surf_GFCs137_lite.mp4"/> |


### 2.2. Model validation

#### 2.2.1 Spatial distribution

|  | Tc-99 (all basins) | I-129 (all basins) |
| --- | --- | --- |
| **Spatial distribution** | ![](../03_data_analysis/01_data_visualisation/04_plot/hist_trc_valid_spat_RPTc99.bmp) | ![](../03_data_analysis/01_data_visualisation/04_plot/hist_trc_valid_spat_RPI129.bmp) |
| **Observation vs. simulation** | ![](../03_data_analysis/01_data_visualisation/04_plot/hist_trc_valid_all_Tc99.bmp) | ![](../03_data_analysis/01_data_visualisation/04_plot/hist_trc_valid_all_I129.bmp) |
| **Mean normalized bias** | **Overall (n=2238): 33.8%** <ul><li>Baltic Sea (n=480): 63.2% <li>Arctic Ocean (n=134, outliers excluded): 43.3% <li>**Nordic Seas (n=612): 3.4%** <li>North Atlantic (n=1011, outliers excluded): 39.1% | **Overall  (n=852): 11.2%** <ul><li>Baltic Sea (n=92): 45.3% <li>Arctic Ocean (n=323, outliers excluded): -38.8% <li>**Nordic Seas (n=179): 23.9%** <li>North Atlantic (n=225, outliers excluded): 73.6% |
| **Correlation coefficient** | **Overall (n=2238): 0.427** <ul><li>Baltic Sea (n=480): 0.427 <li>Arctic Ocean (n=134, outliers excluded): 0.906 <li>**Nordic Seas (n=612): 0.812** <li>North Atlantic (n=1011, outliers excluded): 0.292 | **Overall  (n=852): 0.795** <ul><li>Baltic Sea (n=92): 0.531 <li>Arctic Ocean (n=323, outliers excluded): 0.529 <li>**Nordic Seas (n=179): 0.830** <li>North Atlantic (n=225, outliers excluded): 0.757 |

|  | I-129 (North Atlantic) | I-129 (Arctic Ocean) |
| --- | :---: | :---: |
| **Latitude** | ![](../03_data_analysis/01_data_visualisation/04_plot/hist_trc_valid_NA_Latitude_I129.bmp) | ![](../03_data_analysis/01_data_visualisation/04_plot/hist_trc_valid_AO_Latitude_I129.bmp) |
| **Longitude** | ![](../03_data_analysis/01_data_visualisation/04_plot/hist_trc_valid_NA_Longitude_I129.bmp) | ![](../03_data_analysis/01_data_visualisation/04_plot/hist_trc_valid_AO_Longitude_I129.bmp) |
| **Depth** | ![](../03_data_analysis/01_data_visualisation/04_plot/hist_trc_valid_NA_Depth_I129.bmp) | ![](../03_data_analysis/01_data_visualisation/04_plot/hist_trc_valid_AO_Depth_I129.bmp) |
| **Year** | ![](../03_data_analysis/01_data_visualisation/04_plot/hist_trc_valid_NA_Year_I129.bmp) | ![](../03_data_analysis/01_data_visualisation/04_plot/hist_trc_valid_AO_Year_I129.bmp) |
| **Month** | ![](../03_data_analysis/01_data_visualisation/04_plot/hist_trc_valid_NA_Month_I129.bmp) | ![](../03_data_analysis/01_data_visualisation/04_plot/hist_trc_valid_AO_Month_I129.bmp) |

**Summary:**

1. NorESM has the best performance in the Nordic Seas (low MNB and high r);
2. High NBs and low r are observed in the European marginal seas, such as the Danish Straits and the British coast 
3. Low NBs are observed in the deep water of the Canada Basin (advection or ventilation issue?).

#### 3.2.2 Temporal evolution

|  | Tc-99 | I-129 |
| --- | --- | --- |
| **Station location** | ![](../03_data_analysis/01_data_visualisation/04_plot/hist_trc_timser_st_loci_Tc99.bmp) | ![](../03_data_analysis/01_data_visualisation/04_plot/hist_trc_timser_st_loci_I129.bmp) |
| **Temporal evolution** | ![](../03_data_analysis/01_data_visualisation/04_plot/hist_trc_timser_Tc99.bmp) | ![](../03_data_analysis/01_data_visualisation/04_plot/hist_trc_timser_I129.bmp) |
| **Mean normalized bias** | <li>Danish Straits surf. (n=164): 39.7% <li>Danish Straits bo. (n=37): -19.2% <li>SW Norwegian Coast (n=81): 28.9% <li>NW Norwegian Coast (n=159): -38.3% <li>Barent Sea (n=42): 35.8% <li>Denmark Strait (n=33): -11.3% | <li>Danish Straits surf.(n=46): -23.2% <li>SW Norwegian Coast (n=19): -12.9% |
| **Correlation coefficient** | <li>Danish Straits surf. (n=164): 0.166 <li>Danish Straits bo. (n=37): 0.428 <li>SW Norwegian Coast (n=81): 0.418 <li>NW Norwegian Coast (n=159): 0.753 <li>Barent Sea (n=42): 0.681 <li>Denmark Strait (n=33): not corr. | <li>Danish Straits surf.(n=46): 0.753 <li>SW Norwegian Coast (n=19): 0.923 |

**Summary:**

1. Low r are observed at the stations of the European marginal seas.
2. MNBs are acceptable at all stations;

### 3.3 Point-source releases

#### 3.3.1 Spatial distribution

|  | Surf. tracer age | Surf. transfer factor (no decay) |
| --- | --- | --- |
| **Sellafield** | ![](../03_data_analysis/01_data_visualisation/04_plot/hist_ps_age_surf_RPSF_2018-12.bmp) | ![](../03_data_analysis/01_data_visualisation/04_plot/hist_ps_dil_surf_RPSF_2018-12.bmp) |
| **La Hague** | ![](../03_data_analysis/01_data_visualisation/04_plot/hist_ps_age_surf_RPLH_2018-12.bmp) | ![](../03_data_analysis/01_data_visualisation/04_plot/hist_ps_dil_surf_RPLH_2018-12.bmp) |
| **Fukushima** | ![](../03_data_analysis/01_data_visualisation/04_plot/hist_ps_age_surf_FKFK_2018-12.bmp) | ![](../03_data_analysis/01_data_visualisation/04_plot/hist_ps_dil_surf_FKFK_2018-12.bmp) |

#### 3.3.2 Temporal evolution

|  | Surf. tracer age | Surf. transfer factor (no decay) |
| --- | --- | --- |
| **Station location** | ![](../03_data_analysis/01_data_visualisation/04_plot/hist_ps_timser_st_loci.bmp) | ![](../03_data_analysis/01_data_visualisation/04_plot/hist_ps_timser_st_loci.bmp) |
| **Danish Straits** | ![](../03_data_analysis/01_data_visualisation/04_plot/hist_ps_age_timser_1.bmp) | ![](../03_data_analysis/01_data_visualisation/04_plot/hist_ps_dil_timser_1.bmp) |
| **SW Norwegian Coast** | ![](../03_data_analysis/01_data_visualisation/04_plot/hist_ps_age_timser_2.bmp) | ![](../03_data_analysis/01_data_visualisation/04_plot/hist_ps_dil_timser_2.bmp) |
| **NW Norwegian Coast** | ![](../03_data_analysis/01_data_visualisation/04_plot/hist_ps_age_timser_3.bmp) | ![](../03_data_analysis/01_data_visualisation/04_plot/hist_ps_dil_timser_3.bmp) |
| **Barent Sea** | ![](../03_data_analysis/01_data_visualisation/04_plot/hist_ps_age_timser_4.bmp) | ![](../03_data_analysis/01_data_visualisation/04_plot/hist_ps_dil_timser_4.bmp) |
| **E Fram Strait** | ![](../03_data_analysis/01_data_visualisation/04_plot/hist_ps_age_timser_5.bmp) | ![](../03_data_analysis/01_data_visualisation/04_plot/hist_ps_dil_timser_5.bmp) |
| **W Fram Strait** | ![](../03_data_analysis/01_data_visualisation/04_plot/hist_ps_age_timser_6.bmp) | ![](../03_data_analysis/01_data_visualisation/04_plot/hist_ps_dil_timser_6.bmp) |
| **E Greenland Coast** | ![](../03_data_analysis/01_data_visualisation/04_plot/hist_ps_age_timser_7.bmp) | ![](../03_data_analysis/01_data_visualisation/04_plot/hist_ps_dil_timser_7.bmp) |
| **S Greenland Coast** | ![](../03_data_analysis/01_data_visualisation/04_plot/hist_ps_age_timser_8.bmp) | ![](../03_data_analysis/01_data_visualisation/04_plot/hist_ps_dil_timser_8.bmp) |

**Summary:**

1. Dischages from La Hague has 1 year more transit tiem than thoes from Sellafield.
2. A branch of Sellafield discharges transport across the North Atlantic reaching S Greenland directly.

### 3.5 Water masses in Arctic (to be updated)

### 3.6  U-236 discharge data

#### 3.6.1 Current discharge data

|  | Sellafield | La Hague |
| --- | --- | --- |
| **Discharge data** | ![](../03_data_analysis/01_data_visualisation/04_plot/hist_trc_U236_disch_SF.bmp) | ![](../03_data_analysis/01_data_visualisation/04_plot/hist_trc_U236_disch_LH.bmp) |
| **Data Source** | <li> 1971-1976: shell data <li> 1977-1984: interpolation <li> 1985-2018: shell data | <li> 1966-1996: HELCOM <li> 1997-2018: shell data |
| **Sampling station** | ![](../03_data_analysis/01_data_visualisation/04_plot/hist_trc_timser_st_loci_U236_1.bmp) | ![](../03_data_analysis/01_data_visualisation/04_plot/hist_trc_timser_st_loci_U236_2.bmp) |
| **Temporal evolution** | ![](../03_data_analysis/01_data_visualisation/04_plot/hist_trc_timser_U236_1.bmp) | ![](../03_data_analysis/01_data_visualisation/04_plot/hist_trc_timser_U236_2.bmp) |
| **Mean normalized bias** | <li>Irish Sea: -48% | <li>Wadden Sea: 30.9% | 
| **Correlation coefficient** | <li>Irish Sea: 0.892 | <li>Wadden Sea: 0.706 |


#### 3.6.2 Validation with seaweed data

|  | U-236 |
| --- | --- |
| **Station location** | ![](../03_data_analysis/01_data_visualisation/04_plot/hist_trc_timser_st_loci_U236_3.bmp) |
| **Temporal evolution** | ![](../03_data_analysis/01_data_visualisation/04_plot/hist_trc_timser_U236_3.bmp) |
| **Mean normalized bias** | <li>Danish Straits: 125% |
| **Correlation coefficient** | <li>Danish Straits: 0.829 |

**Summary:**

* La Hague: 
 1. Before 1980: the reconstruted discharge data is more reliable than the official discharge data;
 2. After 1980: the reconstruted discharge data and the official discharge data are consistent with each other.
* Sellafield
 1. Years with shell data are trustable;
 2. The interpolated data may not be right;
 3. Combining transit time and transfer factor results from virtual tracers, it is possible to resolve SF discharge with seaweed data.

## 4. Next Step

1. Re-run WP1 for the vitual tracers of AO water masses;
2. Re-run WP1 for U-236 discharges from RPs;
2. Move on to WP2.
