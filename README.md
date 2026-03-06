# Vegetation data of long-term monitoring in alpine/high-mountain areas following the GLORIA multi summits approach 

## GLORIA Taiwan vegetation data
2026-03-06 version 1.3 (by Cheng-Tao Lin chengtaolin@ntu.edu.tw) 


Progress Overview:
Finished the fourth survey: TW-DAS, TW-SYU
Finished the third survey: TW-NAH (est. finishing the fourth survey around July, 2025), TW-HQM (est. finishing the fourth survey around July, 2025), TW-SAC  (est. finishing the fourth survey around August, 2026)

## Dataset download

[Taiwan_GLORIA_vegetation_data](https://docs.google.com/spreadsheets/d/1tQU7Os3j1JszbFQ1-pM4B1PW17Zxha3747VI2XFPySQ/edit?gid=1499846964#gid=1499846964) (please request for permission)

### Table description
#### 00_plot_coordinates
Stores the geographic and topographic metadata for each summit, including both global (WGS84) and Taiwan local (TWD97) coordinates. This forms the geospatial backbone of all summit-level observations and is essential for mapping and spatial analyses.

#### 01_summits_survey_info
Contains metadata for each summit survey cycle, including survey dates, associated field forms (overview, temperature loggers, vegetation data), and summary comments. It links the temporal structure of the GLORIA monitoring framework.

#### 02_p5_p10m_direction
Describes the spatial arrangement of quadrats and survey points around each summit, including their distance and direction from summit center, cardinal aspect, and coordinate location. It supports analysis of plot orientation and microhabitat positioning.
10_1x1m_plotinfo
Records static physical properties of each 1×1 m quadrat, such as slope and azimuth. It provides the baseline structural information needed to contextualize vegetation and disturbance data at the microhabitat scale.

#### 11_1x1m_env
Summarizes environmental cover types within each 1×1 m quadrat for a specific monitoring cycle, including vascular plant cover, substrate types. It also includes species richness and field notes.

#### 12_1x1m_sp
Lists all species observed in each 1×1 m quadrat, with associated cover percentages and total point-intercept hits. It links species identity with fine-scale plot composition and uses standardized taxon codes (spCode).

#### 13_1x1m_sp_freq (still digitizing)
Provides detailed subquadrat presence/absence (in a 10×10 grid) for each species in each 1×1 m plot. This fine-resolution spatial data enables pattern analysis of microdistribution and overlap among species.

#### 14_1x1m_disturbance
Logs animal disturbance signals (e.g., droppings, browsing, trampling) in each quadrat. Like the species frequency table, it uses a 10×10 grid to map the spatial distribution of disturbances.

#### 21_sas_env
Documents environmental cover estimations for each Summit Area Section (SAS) subquadrat, including substrate and vegetation components. It also records total species counts and any field observations.

#### 22_sas_sp
Presents a presence–abundance species list for each SAS plot, assigning each taxon a Braun-Blanquet abundance class (e.g., rare, common, dominant), both in letter and numeric form. This supports compositional summaries across subplots.

#### 31_10x10m_env
Contains visual estimates of environmental cover types and total species richness for larger 10×10 m plots located on the summit’s four aspects. These plots integrate vegetation structure and substrate information at a broader spatial scale.

#### 32_10x10m_sp
Provides frequency-based species data (i.e., point-intercept hits) from the 10×10 m plots. It complements the 10x10_env table by quantifying species dominance in each plot.

#### 33_sas_abundanceCode
A lookup reference that converts Braun-Blanquet abundance codes (e.g., r, c, d) into numeric values, enabling consistent statistical treatment of ordinal data.

#### 41_speciesList
Acts as a taxonomic authority file for the dataset. It links shorthand species codes (sp_code2) to vernacular names, scientific names, family, IUCN status, endemism, and GBIF references. Essential for taxon standardization and cross-table integration.

#### 42_gbif_checked
Stores results from GBIF taxonomic name matching using nomenMatch (http://match.taibif.tw). It includes original names, matched accepted names, GBIF IDs, hierarchical taxonomy, and quality flags. Used for validating species lists and resolving synonyms.

#### 51_ListContributors
List of the contributors
