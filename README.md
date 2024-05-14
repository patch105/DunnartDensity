# DunnartDensity

<a href="https://zenodo.org/doi/10.5281/zenodo.11189996"><img src="https://zenodo.org/badge/787285575.svg" alt="DOI"></a>

The Julia Creek Dunnart (_Sminthopsis douglasi_) is an endangered small mammal found in central west Queensland, Australia. This project aims to provide the first population density and population size estimates for _S. douglasi_ within a national park. Density and population size are estimated via spatially explicit capture-recapture, using live capture data collected over seven trapping sessions between 2022 and 2023.  

Code and data provided here outline the analysis of _S. douglasi_ capture-recapture data. 

Further details of the project methods, results, and discussion are presented in our paper entitled: "Density of a cryptic Australian small mammal: the threatened Julia Creek Dunnart (_Sminthopsis douglasi_)" Ecology and Evolution. A. H. Bakker, Patterson C.R., Mifsud G., Reside A., Fuller S., and Baker A.M.

The data/code presented here include:
- captfile_zeros.txt : The capture-recapture data from the two trapping grids (Scrammy - Site A and Campbells - Site B), including individual animal IDs, the occasion (trap night), and the detector (trap) that the animal was caught in
- trapfile_campbells_MGA2020.txt : The coordinates of traps in the campbells grid (Site B) in the GDA 2020 / MGA 2020 Zone 55 projection (EPSG:7855). The 'Detector' column matches the IDs within the captfile.  
- trapfile_scrammy_MGA2020.txt : The coordinates of traps in the scrammy grid (Site A) in the GDA 2020 / MGA 2020 Zone 55 projection (EPSG:7855). The 'Detector' column matches the IDs within the captfile.
- AOI_DISSOLVED.shp (and associated files) : The shapefile for the habitat mask, used to calculate the population size of _S. douglasi_ within Bladensburg National Park.
- covariates.csv : The Site and Season covariates for the Site and Season models. Ordered by the order that sessions are loaded into the capthist object in secr (alphabetical session names). 
- Dunnar_Density.qmd : All code used to run the spatially explicit capture-recapture analysis within a Quarto document.
- Dunnart_Density.html : All code used to run the spatially explicit capture-recapture analysis in html format.
- Dunnart_Density.RPROJ : The associated R project for the analysis.

Contact Charlotte Patterson at crpattrsn@gmail.com for queries.
