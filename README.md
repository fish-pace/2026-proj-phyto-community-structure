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
    * Massachussets Bay: *Pseudo-nitzschia* bloom, June 16-19, 2025
    * Chesapeake Bay:
        * *Levanderina fissa* bloom, July 22, 2025
        * *Heterocapsa rotundata* bloom, August 27, 2024
    * West Florida Shelf: *Karenia brevis* bloom, October 2024

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
* State phytoplankton monitoring data
    * Massachusetts (MA)
    * Maryland/Virginia (MD/VA)
    * Florida (FL)

* OLCI imagery
    * Used for identifying bloom timing, spatial extent, and selecting cloud-free PACE overpasses
 
* PACE OCI imagery
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
        * Pre-bloom: Sept 23, 2024)
        * Post-bloom (Oct 21, 2024)
    * FWC has field data

* Massachusetts Bay
    * *Pseudo-nitzschia* bloom, June 16-19, 2025
    * Bounding box for Massachusetts Bay: -71.7 to -67.8 and 40.6 to 43.5

## Tasks:
1/29: 
MA: Plots are done (AVW, Chla, spectra from Rrs)
Learned how to use PACE code rather than SeaDAS  
Changes at start or end of field date
Devon add slide for MA with purpose statement 
Chesapeake: Chla, AVW done (from Rrs). Not great due to high Rrs and chl. Can look into using Rhos (Shelly). Sachi working on capturing spectra. Would suggest using the Rhos from SFREFL files rather than the AOP (Rrs).
FL: Felix use Cassie’s code to do a similar analysis for Karenia 

Extract standard imagery products for:
Massachusetts Bay: Jun 16 or 19, 2025 - Devon/Cassandra
Chesapeake Bay: Aug 27, 2024 Heterocapsa or July 21, 2025 Levanderina blooms - Shelly
West Florida Coast: October 23, 2024 - Felix
Pull PACE dataset - https://search.earthdata.nasa.gov/search?fi=OCI
Collect in-situ cell count data
Look at transect across Florida Karenia brevis bloom - Felix
Chesapeake Bay
Extract points from field dataset in Chesapeake Bay - Sachi
Massachusetts Bay, Jun 17, 2025, MWRA field survey
Analyze imagery for remote sensing reflectance
Compare against known group standards

## Approach: 
Exploratory: Select 3 blooms
Look at spectra for certain blooms and see if they are different for 3 blooms
Look at existing algorithms, how could they be tweaked, modified
Cassandra - has code already for extracting spectra from her zooplankton work that could be used to investigate differences in these blooms. 

## Results/Findings

## Lessons Learned

## References

