This repo is for a Django app that enables manual curation of the mapping of small molecule binding to Pfam-A domains described in an [InCoB 2012 conference supplement](http://www.biomedcentral.com/bmcbioinformatics/supplements) onto the target dictionary of a given ChEMBL release. Manual curation assignments can be made using a web-interface and are stored in a table *pfam_maps* that was added to the default ChEMBL schema. Manual assigments can be exported using the exporter script
in the [pfam_map_loader]{https://github.com/fak/pfam_map_loader} repo. Uncurated mappings rely on the projection of protein domains with known small molecule interactions, while curated mappings are carried over to the next release.

This is to replace an older mechanism that generated mappings for each release of the ChEMBL database but needed to be adjusted with the schema change that occurred at the transition between chembl_14 and  chembl_15. Mappings of older versions are provided on a dedicated [website](http://www.ebi.ac.uk/~fkrueger/mapChEMBLPfam/).
