# **GRSciColl refinements**

## RBINS - RMCA collections

### Adjusting values of DwC terms in already published datasets

GBIF recommended guidelines for specimen-related occurrence records: 

https://scientific-collections.gbif.org/connected-systems#occurrences-published-on-gbif

* to optimise relevant data aggregation in GRSciColl collections 
* to avoid issued flags - https://data-blog.gbif.org/post/grscicoll-flags/

Technical methods for these refinements via https://ipt.biodiversity.be/manage/: 

* OpenRefine = possible for ds:
	- Therevidae ds (collectionCode: INV-ENT --> INV-INS)
	- Bees ds (")
	- Moths ds (") 
	- MODIRISK:RBINS Diptera: Culicidae Collection or alt. method w/ R  (")

* Rscript + github
	MODIRISK:RBINS Diptera: Culicidae Collection: possibly appropriate to keep track of adjustements in the ITG repo:
	https://github.com/BelgianBiodiversityPlatform/data-publication-ITG/blob/master/datasets/modirisk-occurrences/scr/dwc_mapping_collections_patch_grscicoll.Rmd 

* SQL db:
	- Beetles (")
	- Ants Chaco  (")
	- Ants formidabel (", also change institutionCode: KBVE-SRBE --> RBINS)
	- African Mammalia (collectionCode: Rodentia --> VER-MAM)
	- RMCA Metafro-Infosys - Xylarium (just shorten the institutionCode into RMCA)
