[![DOI](https://zenodo.org/badge/596931005.svg)](https://doi.org/10.5281/zenodo.14866008)

# L-RNA Aptamer-Based CXCL12 Inhibition Combined with Radiotherapy in Newly Diagnosed Glioblastoma: Dose Escalation of the Phase I/II GLORIA Trial

### [Published in Nature Communications](https://doi.org/10.1038/s41467-024-48416-9) 

## Authors & Affiliations

**Frank A. Giordano**<sup>1,2,13</sup>, **Julian P. Layer**<sup>3,4,13</sup>, **Sonia Leonardelli**<sup>4,13</sup>, **Lea L. Friker**<sup>4,5</sup>, **Roberta Turiello**<sup>4</sup>,  **Dillon Corvino**<sup>4</sup>, **Thomas Zeyen**<sup>6</sup>, **Christina Schaub**<sup>6</sup>, **Wolf Müller**<sup>7</sup>, **Elena Sperk**<sup>1</sup>, **Leonard Christopher Schmeel**<sup>3</sup>, **Katharina Sahm**<sup>2,8,9</sup>, **Christoph Oster**<sup>10</sup>, **Sied Kebir**<sup>10</sup>, **Peter Hambsch**<sup>11</sup>, **Torsten Pietsch**<sup>5</sup>, **Sotirios Bisdas**<sup>12</sup>, **Michael Platten**<sup>2,8,9</sup>, **Martin Glas**<sup>10</sup>, **Clemens Seidel**<sup>11</sup>, **Ulrich Herrlinger**<sup>6,13</sup>, **Michael Hölzel**<sup>4,13</sup>
 
<sup>1</sup> Department of Radiation Oncology, University Medical Center Mannheim, Medical Faculty Mannheim, University of Heidelberg, Mannheim, Germany  
<sup>2</sup> DKFZ Hector Cancer Institute at the University Medical Center Mannheim, Mannheim, Germany  
<sup>3</sup> Department of Radiation Oncology, University Hospital Bonn, University of Bonn, Bonn, Germany  
<sup>4</sup> Institute of Experimental Oncology, Medical Faculty, University Hospital Bonn, University of Bonn, Bonn, Germany  
<sup>5</sup> Institute of Neuropathology, University Hospital Bonn, University of Bonn, Bonn, Germany  
<sup>6</sup> Department of Neurooncology, Center for Neurology, University Hospital Bonn, Bonn, Germany  
<sup>7</sup> Institute of Neuropathology, University Hospital Leipzig, University of Leipzig, Leipzig, Germany  
<sup>8</sup> Department of Neurology, Medical Faculty Mannheim, MCTN, Heidelberg University, Mannheim, Germany  
<sup>9</sup> DKTK Clinical Cooperation Unit Neuroimmunology and Brain Tumor Immunology, German Cancer Research Center, Heidelberg, Germany  
<sup>10</sup> Division of Clinical Neurooncology, Department of Neurology, Center for Translational Neuro- and Behavioral Sciences (C-TNBS) and West German Cancer Center, German Cancer Consortium, Partner Site Essen, University Hospital Essen, University Duisburg-Essen, Essen, Germany  
<sup>11</sup> Department of Radiation Oncology, University Hospital Leipzig, University of Leipzig, Leipzig, Germany  
<sup>12</sup> Lysholm Department of Neuroradiology, University College London, London, UK  

<sup>13</sup> Authors contributed equally: **Frank A. Giordano, Julian P. Layer, Sonia Leonardelli, Ulrich Herrlinger, Michael Hölzel**  

## Contact Information  

**Correspondence:** [Frank.Giordano@umm.de](mailto:Frank.Giordano@umm.de), [michael.hoelzel@ukbonn.de](mailto:michael.hoelzel@ukbonn.de)  

---

## Abstract

The chemokine CXCL12 promotes glioblastoma (GBM) recurrence after radiotherapy (RT) by facilitating vasculogenesis. Here, we report outcomes of the dose-escalation part of GLORIA (NCT04121455), a phase I/II trial combining RT and the CXCL12-neutralizing aptamer olaptesed pegol (NOX-A12; 200/400/600 mg per week) in patients with incompletely resected, newly diagnosed GBM lacking MGMT methylation.  

The primary endpoint was safety; secondary endpoints included maximum tolerable dose (MTD), recommended phase II dose (RP2D), NOX-A12 plasma levels, topography of recurrence, tumor vascularization, neurologic assessment in neuro-oncology (NANO), quality of life (QOL), median progression-free survival (PFS), 6-months PFS, and overall survival (OS).  

Treatment was safe, with no dose-limiting toxicities or treatment-related deaths. The MTD was not reached, and 600 mg per week of NOX-A12 was established as the RP2D for the ongoing expansion part of the trial. With increasing NOX-A12 dose levels, a corresponding increase in NOX-A12 plasma levels was observed. Of ten patients enrolled, nine showed radiographic responses, and four reached partial remission.  

All but one patient (90%) showed reduced perfusion values in terms of relative cerebral blood volume (rCBV). The median PFS was 174 (range 58-260) days, 6-month PFS was 40.0%, and the median OS was 389 (144-562) days. In a post-hoc exploratory analysis of tumor tissue, a higher frequency of CXCL12+ endothelial and glioma cells was significantly associated with longer PFS under NOX-A12.  

Our data imply the safety of NOX-A12, and its efficacy signal warrants further investigation.

---

## Dataset Info 

As part of this study, we reanalyzed **Single-cell analysis of human glioma and immune cells identifies S100A4 as an immunotherapy target**, Abdelfattah, et al., 2022, *Nature Communications* 13, 767 ([doi:10.1038/s41467-022-28372-y](https://doi.org/10.1038/s41467-022-28372-y); GEO [GSE182109](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE182109)).  

- Data was downloaded from the **Single Cell Portal** (Broad Institute).  
- For further details on the original dataset and associated code, refer to the **[GBMatlas GitHub repository](https://github.com/parveendabas/GBMatlas)**.  
- The reprocessed Seurat object (`GBM_seurat_object.h5seurat`) is **not stored in this repository** — it is derived from the public Abdelfattah et al. (GSE182109) data and can be regenerated from that source using the scripts here.  

---

## Repository structure

```
scripts/01_GBM_Dataset.Rmd   # reanalysis of the public glioma single-cell atlas: CXCL12-positive cells across cell types and clusters
results/figures/             # Fig 3A, Supplementary Fig 3 and the underlying cell-count tables
```

## Reproducing the analysis

1. Download the glioma single-cell atlas from the Broad Single Cell Portal (see [Dataset Info](#dataset-info); accession GSE182109).
2. Knit `scripts/01_GBM_Dataset.Rmd` from the repository root. The notebook sets its working directory with `here::here()` and loads its packages in the Setup chunk.

The same public dataset is also reprocessed, with a general preprocessing workflow, in [`tumour-immune-scrnaseq-reanalyses`](https://github.com/Eomesodermin/tumour-immune-scrnaseq-reanalyses/tree/main/datasets/abdelfattah_2022).


## Citation

To cite the paper, use the DOI above; to cite this code, use the Zenodo DOI in the badge at the top. Machine-readable citation metadata is in [`CITATION.cff`](CITATION.cff).

---

## Code Attribution  

This code and analysis were authored by **Dillon Corvino** — [github.com/Eomesodermin](https://github.com/Eomesodermin) · [dilloncorvino.com](https://dilloncorvino.com).  
