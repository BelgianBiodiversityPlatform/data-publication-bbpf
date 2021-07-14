# Data publication Florient Atlas uGent

## Rationale

This repository contains the functionality to standardize the Florient dataset **Florient wild flora occurrences** to [Darwin Core Occurrence](https://www.gbif.org/dataset-classes) datasets that can be harvested by [GBIF](http://www.gbif.org). 

## Datasets

Title (and GitHub directory) | IPT | GBIF
--- | --- | --- 
[Florient wild flora occurrences](datasets/florient) | [Florient wild flora occurrences](https://ipt.biodiversity.be/resource?r=%%%%%%%%) | <https://doi.org/%%%%%%> |


## Repo structure

The structure for each dataset in [datasets](datasets) is based on [Cookiecutter Data Science](http://drivendata.github.io/cookiecutter-data-science/) and the [Checklist recipe](https://github.com/trias-project/checklist-recipe). Files and directories indicated with `GENERATED` should not be edited manually.

```
├── data
│   ├── raw                  : Source data, input for mapping script
│   ├── interim              : Derived data for verification GENERATED
│   └── processed            : Darwin Core output of mapping script GENERATED
│
├── src
│   └── dwc_mapping.Rmd      : Darwin Core mapping script
│
└── specs
    └── dwc_occurrences.yaml : Whip specifications for validation
```

## Contributors

[List of contributors](*******)

## License

[MIT License](LICENSE) for the code and documentation in this repository. The included data is released under another license.
