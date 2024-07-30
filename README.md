# Code for generating data, figures used in the SCUBA manuscript

<!-- Click here to view the manuscript. --> <!-- Link to manuscript -->

To run the code in the Rmd files included in this repo, SCUBA and all dependencies must be installed. For more information, see the "Pre-requisites" and "Installation" sections of the [SCUBA repo README](https://github.com/amc-heme/SCUBA).

## Data

The objects used for demonstration in the SCUBA manuscript exists in the [SCUBA](https://github.com/amc-heme/SCUBA) repo and can be accessed by calling `library(SCUBA)` and then running one of the three functions below.

The objects were derived from the Accute Myeloid Leukemia (AML) reference dataset created by [Triana et al. 2021](https://doi.org/10.1038/s41590-021-01059-0). [`Demo_Object_Generation.Rmd`](https://github.com/amc-heme/SCUBA_Manuscript/blob/main/Demo_Object_Generation.Rmd) contains all code needed to generate each of the three objects from the inital dataset. 

```
# Seurat Object
AML_Seurat

# SingleCellExperiment Object
AML_SCE()

# anndata object
AML_h5ad()
```

## Contents

- [`Demo_Object_Generation.Rmd`](https://github.com/amc-heme/SCUBA_Manuscript/blob/main/Demo_Object_Generation.Rmd): code for generating the `AML_Seurat`, `AML_SCE()`, and `AML_h5ad()` datasets from the Triana et al. 2021 reference dataset.
- [`Fig2.Rmd`](https://github.com/amc-heme/SCUBA_Manuscript/blob/main/Fig2.Rmd): examples of FetchData methods added by SCUBA for SingleCellExperiment and anndata objects alongside the existing Seurat method, as shown in Figure 2 of the manuscript.
- [`Fig3.Rmd`](https://github.com/amc-heme/SCUBA_Manuscript/blob/main/Fig3.Rmd): examples of `fetch_metadata` and `fetch_reduction` generics created by SCUBA for the retrieval of metadata and reductions, repsectively.
- [`Fig4.Rmd`](https://github.com/amc-heme/SCUBA_Manuscript/blob/main/Fig4.Rmd): code used to evaluate performance of FetchData on a large multimodal reference dataset.
- [`Fig5.Rmd`](https://github.com/amc-heme/SCUBA_Manuscript/blob/main/Fig5.Rmd): code demonstrating the use of SCUBA methods as a foundation for plotting.
- [`Fig6.Rmd`](https://github.com/amc-heme/SCUBA_Manuscript/blob/main/Fig6.Rmd): example usage of SCUBA to view the unique values of a metadata variable in an object, a common object exploration operation.
