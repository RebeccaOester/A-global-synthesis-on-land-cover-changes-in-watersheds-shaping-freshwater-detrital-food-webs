# A-global-synthesis-on-land-cover-changes-in-watersheds-shaping-freshwater-detrital-food-webs

READ ME

Rebecca Oester, François Keck, Marcelo S. Moretti, Florian Altermatt, Andreas Bruder, Verónica Ferreira

Rebecca.oester@eawag.ch

This READ ME file contains information on the r-scripts and variables in the datasets used for the analyses.

Datafiles:

dat.MA: Main dataset with information on each observation of each study with the following variables:

study_ID		Levels: several; unique identifier for each study
ID			Levels: continuous: unique identifier for each comparison
year			Levels: continuous, publication year
lat			Levels: continuous; latitude in decimal degrees
lon			Levels: continuous; longitude in decimal degrees
climate			Levels: boreal, temperate; sub-tropical, tropical, climate zone
season			Levels: year, winter, spring, summer, autumn, dry, wet; timepoint of field study
scale			Levels: local, catchment, local+catchment; spatial scale of field study
temp_diff		Levels: continuous; temporal difference between before and after comparison in days
space_diff		Levels: continuous; spatial difference between refernce and altered comparison in meters
duration		Levels: continuous; duration of decomposition assays in days
water_body		Levels: several; type of water body, e.g., stream
strahler		Levels: continuous; Strahler order
veg_change		Levels: several; type of vegetation change according to authors
width_ref		Levels: continuous; m width of riparian vegetation in the reference condition
width_alt		Levels: continuous; m width of riparian vegetation in the altered condition
cover_ref		Levels: continuous; % cover of refernence vegetation of riparian vegetation in the reference 			condition
cover_alt		Levels: continuous; % cover of refernence vegetation of the reference condition
veg_ref			Levels: several; characterisation of reference vegetation and land cover
veg_alt			Levels: several; characterisation of altered vegetation and land cover
fw_category		Levels: 1-6; 1= detritus, 2= microbes, 3= macroinvertebrates+fish, 4= microbial 				decomposition, 5= shredder-mediated decomposition, 6= total decomposition
fct_group		Levels: 1-3, functional group with 1= detritus, 2= microbes, 3= macroinvertebrates+fish
om_type			Levels: several, organic matter type, e.g., leaf
om_taxon		Levels: several, taxon name for organic matter
microbe_type		Levels: several, type of microbe, e.g., bacteria
invert_type		Levels: several, type of invertebrate, e.g., macroinvertebrate
compartment_type	Levels: CPOM, benthic, water column  where organisms where collected
metric			Levels: abundance, diversity, biomass, decomposition as ecosystem and community metrics
unit			Levels: several; unit in which metric was reported
mean_ref		Levels: continuous; mean reference value of this comparison
mean_alt		Levels: continuous; mean altered value of this comparison
n_ref			Levels: continuous; number of replications in reference condition of this comparison
n_alt			Levels: continuous; number of replications in altered condition of this comparison
origin			Levels: several; data origin description
dataorigin		Levels: reported = either text, table or provided by authors, estimated= from figure 				extracted 
trophy			Levels: 1-4; 1= detritus, 2= microbes, 3= shredders, 4= omnivores
Imputed_Value_ref	Levels: continuous; if imputed, new value for reference condition
Imputed_Value_alt	Levels: continuous; if imputed, new value for altered condition
sd_ref3			Levels: continuous; standard deviation of reverence value of this comparison
sd_alt3			Levels: continuous; standard deviation of altered value of this comparison





R-scripts: Run in R (version 4.4.1) on Windows.

1. Data_Distribution: 
requires dat_MA.

Descriptive Analysis of Dataset. Outputs are Manuscript Figures 2 and Figures S8-S10.

2. Data_Analyis_ES:
requires dat_MA.

Main Analysis of Effect Size for each moderator. Otuputs are Tables 1-2, Figures 3-4, and Table S2. 

3. Data_Analyis_Multitropy:
requires dat_MA.

Main Analysis of Effect Size for multitrophic effects. Otuputs are Figure 5. 


4. Data_Analyis_PublicationBias:
requires dat_MA.

Analysis for assessing publication bias. Otuputs are Figures S1-S5 and Table S5. 

5. Data_Analyis_Sensitiviy:
requires dat_MA.

Sensitivity analysis. Otuputs are Figures S6-S7 and Tables S3-S4. 







