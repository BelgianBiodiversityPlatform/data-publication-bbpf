# **GRSciColl refinements**

## Adjusting values of DwC terms in already published datasets

GBIF recommended guidelines for specimen-related occurrence records: 

https://scientific-collections.gbif.org/connected-systems#occurrences-published-on-gbif

* institutionCode: main code for institute in GBIF Registry
* collectionCode: CETAF-DiSSCo-oriented collection coding (cf. comparison)
* institutionID: ROR ID
	* https://discourse.gbif.org/t/preferred-identifiers-for-grscicoll-entries-should-we-mint-dois-for-collections/4403 (Grosjean et al. 2024): The preferred identifiers should be RORs for institutions.
	* https://riojournal.com/article/97374/instance/8199067/ (Agosti et al. 2022): To identify research organisations, ROR is currently the most recommended option.
* collectionID: GRSciColl UUID = UUID by GBIF Registry: is an already applicable, suggested option according to ongoing discourses (beside doi that could be minted in due course)

Main objectives:
* to optimise relevant data aggregation in GRSciColl collections 
* to avoid issued flags - https://data-blog.gbif.org/post/grscicoll-flags/

Technical methods for these refinements via https://ipt.biodiversity.be/manage/: 

### RBINS - RMCA collections

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

### UGent collections

4 essential datafields per specimen-related occurrence record:
- institutionCode = Ugent (ok, already added)
- yet to add ROR ID as institutionID = https://ror.org/00cv9y106 
- possibly yet to refine collectionCode 
- possibly add collectionID
