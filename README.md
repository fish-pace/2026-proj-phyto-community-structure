# Readme For Phytoplankton Community Structure project

**Folder Structure**

* `contributor_folders` (optional) Each contributor can make a folder here and 
push their work here during the week. This will allow everyone to see each others work but prevent any merge conflicts.
* `final_notebooks` When the team develops shared final notebooks, they 
can be shared here. Make sure to communicate so that you limit merge conflicts.
* `scripts` Shared scripts or functions can be added here.
* `data` Shared dataset can be shared here. Note, do not put large datasets on GitHub. Speak to the organizers if you 
need to share large datasets. 

## Project Name: Phytoplankton Community Structure

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


## Planning

### Initial idea:
* We aimed to investigate whether distinct phytoplankton bloom types exhibit measurable differences in hyperspectral reflectance signatures using PACE data.

* Specifically, we examined a few known high-biomass blooms across three regions of the U.S. East Coast: Massachusetts Bay, Chesapeake Bay, and the West Florida Shelf.

* The selected bloom events were:
    * Massachussets Bay: *Pseudo-nitzschia* bloom, June 16-19 2025

* We wanted to investigate if there were differences between a few known high biomass blooms in three regions of the East Coast (Massachusetts, Chesapeake Bay, and the West Florida coast). A bloom of Pseudo-nitzschia was selected for MA Bay June 16-19, 2025; Chesapeake Bay a Levanderina fissa bloom on July 22, 2025 and a Heterocapsa rotundata bloom on August 27, 2024; and West FL coast a Karenia brevis bloom in October 2024. Field data was collected from state monitoring programs in MA, MD, and FL to identify key bloom dates. OLCI and several browsers were used to select clear PACE image dates which coincided with bloom occurrence. We created Chl from standard PACE products to help identify high biomass regions, investigated the use of the AVW (both from RRS and Rhos). The goal of the project was to see if we could see any differences in the spectra of these different bloom formers. 

* Slack channel: proj-phyto-community-structure
* Project google drive: None
* Final presentation: https://docs.google.com/presentation/d/1GYdNin_IicdsqjsnjJLL2Vu7Wsp47_FCp-3Wl_4WwUU/edit?usp=sharing

## Background

## Goals

Examine differences in reflectance spectra between a few high biomass blooms on the East Coast of the US

## Datasets

MD/VA State phytoplankton data
MA State phytoplankton data
FL State phytoplankton data
OLCI imagery to identify potential clear dates for PACE, and bloom extent and timing

## Workflow/Roadmap
Project Idea:
Investigating PACE hyperspectral imagery for harmful algal blooms (HABs) in Massachusetts Bay, Chesapeake Bay and West Florida Shelf.

Study areas:
Chesapeake Bay
	Dataset: MDPhyto_forPACE.xls
	Extracted from MD DNR and VA Department of Health phytoplankton data
Heterocapsa/other - VA/MD dataset (Shelly) -> Mar 10-Apr 16, 2024
Levanderina fissa - Jun 25-Jul 21, 2025
West Florida Shelf - Karenia in 2024 - pre-bloom (Sept 23, 2024), post-bloom (Oct 21, 2024) - FWC has field data
Massachusetts Bay
June 16 - June 19 2025, pseudo-nitzschia
Bounding box for Massachusetts Bay, -71.7 to -67.8 and 40.6 to 43.5

Tasks:
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

Approach: 
Exploratory: Select 3 blooms
Look at spectra for certain blooms and see if they are different for 3 blooms
Look at existing algorithms, how could they be tweaked, modified
Cassandra - has code already for extracting spectra from her zooplankton work that could be used to investigate differences in these blooms. 

## Results/Findings

## Lessons Learned

## References

