# Readme For Phytoplankton Community Structure project

**Folder Structure**

* `contributor_folders` (optional) Each contributor can make a folder here and 
push their work here during the week. This will allow everyone to see each others work but prevent any merge conflicts.
* `final_notebooks` When the team develops shared final notebooks, they 
can be shared here. Make sure to communicate so that you limit merge conflicts.
* `scripts` Shared scripts or functions can be added here.
* `data` Shared dataset can be shared here. Note, do not put large datasets on GitHub. Speak to the organizers if you 
need to share large datasets. 

# Project Name: Phytoplankton Community Structure

## One-line Description

This project looked at spectral differences between 4 blooms along the east coast of the US. 

## Collaborators

| Name                | Role                |
|---------------------|---------------------|
| Participant 1       |Shelly Tomlinson     |
| Participant 2       |Sachi Edirisinghe    |
| Participant 3       |Devon Winkler        |
| Participant 4       |Felix Jose           |
| Participant 5       |Cassandra Pacheco    |


# Planning

## Initial idea:
* We aimed to investigate whether distinct phytoplankton bloom types exhibit measurable differences in hyperspectral reflectance signatures using PACE data.

* Specifically, we examined a few known high-biomass blooms across three regions of the U.S. East Coast: Massachusetts Bay, Chesapeake Bay, and the West Florida Shelf.

* The selected bloom events were:
    * Massachussets Bay:
        * *Pseudo-nitzschia* bloom, June 16-19, 2025
    * Chesapeake Bay:
        * *Levanderina fissa* bloom, July 22, 2025
        * *Heterocapsa rotundata* bloom, August 27, 2024
    * West Florida Shelf:
        * *Karenia brevis* bloom, October 2024

* Field data was collected from state monitoring programs in MA, MD, and FL to identify key bloom dates.

* OLCI imagery and several satellite data browsers were used to identify cloud-free PACE acquisition dates that coincided with bloom events.

* Standard PACE-derived chlorophyll-a (Chl-a) products were generated to help delineate high-biomass regions. We further explored the use of Apparent Visible Wavelength (AVW) derived from both remote sensing reflectance (Rrs) and surface reflectance (Rhos).

* The overarching goal was to assess whether these blooms exhibit distinct spectral signatures, potentially enabling improved discrimination of bloom-forming taxa using hyperspectral satellite observations.


## Project Logistics:
* Slack channel: proj-phyto-community-structure
  
* Project google drive: None
  
* Final presentation: https://docs.google.com/presentation/d/1GYdNin_IicdsqjsnjJLL2Vu7Wsp47_FCp-3Wl_4WwUU/edit?usp=sharing

# Background

## Goals
* To examine whether high-biomass blooms dominated by different phytoplankton taxa exhibit distinct reflectance spectra and AVW characteristics, using PACE hyperspectral imagery combined with *in situ* observations.
  
# Datasets
* State phytoplankton monitoring data:
    * Massachusetts (MA)
    * Maryland/Virginia (MD/VA)
    * Florida (FL)

* OLCI imagery:
    * Used for identifying bloom timing, spatial extent, and selecting cloud-free PACE overpasses
 
* PACE OCI imagery:
    * Hyperspectral remote sensing reflectance (Rrs)
    * Surface Reflectance (Rhos)
    * Derived chlorophyll-a and AVW products

# Workflow/Roadmap
## Project Idea:
Investigate the use of PACE hyperspectral imagery to characterize and compare harmful algal blooms (HABs) in:
* Massachusetts Bay
* Chesapeake Bay
* West Florida Shelf
  
## Study areas and Bloom Events:
* Chesapeake Bay
	* Dataset: MDPhyto_forPACE.xls
	* Extracted from MD DNR and VA Department of Health phytoplankton data
    * Bloom events:
        * *Levanderina fissa* bloom: Mar 10-Apr 16, 2024
        * *Heterocapsa rotundata* bloom: Jun 25-Jul 21, 2025

* West Florida Shelf
    * *Karenia brevis* bloom in 2024
        * Pre-bloom: Sept 23, 2024
        * Post-bloom: Oct 21, 2024
    * FWC has field data

* Massachusetts Bay
    * *Pseudo-nitzschia* bloom, June 16-19, 2025
    * Bounding box for Massachusetts Bay:
        * Latitude: -71.7 to -67.8
        * Longitude: 40.6 to 43.5
    *  Field observations from MWRA surveys

## Tasks:
Extract standard imagery products for:
Massachusetts Bay: Jun 16 or 19, 2025 - Devon/Cassandra
	- Massachusetts Bay, Jun 17, 2025, MWRA field survey
	- Analyze imagery for remote sensing reflectance
	- Compare against known group standards
	- Also looked at the 2nd derivative

Chesapeake Bay: Aug 27, 2024 Heterocapsa or July 21, 2025 Levanderina blooms - Shelly/Sachi
	- Pulled data from MD DNR dataset for both blooms and picked 3 locations
	- Looked at PACE standard Chla, AVW and brightness
	- Values were too high in the Bay, so investigated use of Rhos products
	- Calculate AVW and brightness for Chesapeake
	- Extracted spectra from both Rrs and Rhos
	- Also looked at the 2nd Derivative

West Florida Coast: October 23, 2024 - Felix
	- Pulled field data from FWC
	- Pull PACE dataset - https://search.earthdata.nasa.gov/search?fi=OCI
	-Look at transect across Florida Karenia brevis bloom from offshore to nearshore where bloom was thickest.
	-Also looked at the 2nd Derivative

## Approach: 
Exploratory: Select 3 blooms
For this project, we used a similar approach to compare PACE products and spectra for 2 blooms in Chesapeake Bay, one in MA Bay, and one on the West FL coast. Initially, we all looked at standard PACE products, such as Chla, AVW, and brightness. For MA and FL, we produced spectra to see if there were any differences between a diatom (Pseudo-nitzschia) and a dinoflagellate (Karenia brevis). We also looked at Chesapeake Bay for blooms of Heterocapsa rotundata and Levanderina fissa blooms. Unfortunately, due to issues with using a Case 1 Chla product, and/or issues with the atmospheric correction, we decided to calculate an AVW and brightness from the Rhos in the SFREFL files. We also compared spectra from Rhos vs Rrs, and 2nd derivatives.

## Results/Findings
This was an exploratory project, and no clear results were found. When comparing spectra and 2nd derivative spectra for the 4 blooms, there is no clear difference in spectra that indicate an ability to separate the blooms. In the case of the Karenia brevis bloom in Florida, there were (as expected) clear changes in the spectra and 2nd derivative when looking at a transect of the bloom from clear offshore waters to inshore, where the bloom was dense. In Chesapeake Bay, as has been published elsewhere, the standard Chla was not accurate when compared with validated OLCI red-edge Chla products. This suggest that it might be useful for the PACE program to provide a more accurate Chla product for coastal and estuarine systems. When comparing Rhos to Rrs spectra there are clear issues in the blue bands which indicate the need for an accurate atmospheric correction for standard Case 1 algorithms (CDOM, absorbing aerosols, etc). However, differences were minor in the green to red indicating the value of algorithms in this portion of the spectra in these systems.
When looking at the AVW and brightness in coastal systems, there was not a 1:1 match up with the blooms and these products in Chesapeake Bay. They tended to show a small contrast in the green bands in areas of more turbidity vs. high Chla absorption. However, they seemed to work as expected for the Karenia brevis bloom, and possibly the MA bloom (although we only had samples nearshore where there seemed to be contaminated pixels).

## Lessons Learned
As this was exploratory, we learned to adapt to differences between the 3 regions. There were definitely more issues with traditional products in Chesapeake Bay, compared to Florida and Massachusetts. The key lesson here is that the optical characteristics of a region need to be considered when using PACE products, and in estuarine/Case 2 waters standard products may not be sufficient. Overall, we saw no obvious differences in the spectra from the 4 blooms, however more research would need to be done to determine if separation is possible.

## References
Cannizzaro, JP et al., 2008. A novel technique for detection of the toxic dinoflagellate, Karenia brevis, in the Gulf of Mexico from remotely sensed ocean color data. Continental Shelf Research 28:137–158.
Soto, IM et al., 2015. Evaluation and optimization of remote sensing techniques for detection of Karenia brevis blooms on the West Florida Shelf. Remote Sens. Env. 170:239-254.
Stumpf, RP et al., 2003. Monitoring Karenia brevis blooms in the Gulf of Mexico using satellite ocean color imagery and other data. Harmful Algae 2:147-160.
Stumpf, RP et al., 2008. Hydrodynamic accumulation of Karenia of the west coast of Florida. Continental Shelf Research, 28:189-213.
Wolny, JL et al., 2020. Current and future remote sensing of harmful algal blooms in the Chesapeake Bay to support the shellfish industry. J. Shellfish Res. Front. Mar. Sci. 7:337. doi: 10.3389/fmars.2020.00337
Wynne, TT et al., 2022. Evaluating the Efficacy of Five Chlorophyll-a Algorithms in Chesapeake Bay (USA) for Operational Monitoring and Assessment. J. Mar. Sci. Eng. 2022, 10,
	1104. https://doi.org/10.3390/jmse10081104.

