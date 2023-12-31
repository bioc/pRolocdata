Spatial proteomics datasets
============================

## The `pRolocdata` package

`pRolocdata` is a [Bioconductor](http://bioconductor.org/)
[experiment package](http://bioconductor.org/packages/release/BiocViews.html#___ExperimentData)
([release](http://bioconductor.org/packages/release/data/experiment/html/pRolocdata.html)
and
[devel](http://bioconductor.org/packages/devel/data/experiment/html/pRolocdata.html)
pages) that collects published (mainly, although some unpublished
datasets are also available) mass spectrometry-based spatial/organelle
and protein-complex dataset. The data are distributed as `MSnSet`
instances (see the
[`MSnbase`](http://www.bioconductor.org/packages/release/bioc/html/MSnbase.html)
for details) and are used throughout the
[`pRoloc`](http://bioconductor.org/packages/release/data/experiment/html/pRolocdata.html)
and
[`pRolocGUI`](http://bioconductor.org/packages/devel/bioc/html/pRolocGUI.html)
software for spatial proteomics data analysis and visualisation.

**Current build status**:

[![Build Status](https://travis-ci.org/lgatto/pRolocdata.svg?branch=master)](https://travis-ci.org/lgatto/pRolocdata)

### Installation




```r
if (!requireNamespace("BiocManager", quietly=TRUE))
    install.packages("BiocManager")
BiocManager::install("pRolocdata")
```

Once installed, the package needs to be loaded


```r
library("pRolocdata")
```

### Available datasets

Currently, there are 144 datasets available in
`pRolocdata`. Use the `pRolocdata()` function to obtain a list of data
names and their description.


```r
pRolocdata()
```


|Data                                  |Description                                                                                                                    |
|:-------------------------------------|:------------------------------------------------------------------------------------------------------------------------------|
|Barylyuk2020ToxoLopit                 |Whole-cell spatial proteome of Toxoplasma: molecular anatomy of an apicomplexan cell                                           |
|E14TG2aR                              |LOPIT experiment on Mouse E14TG2a Embryonic Stem Cells from Breckels et al. (2016)                                             |
|E14TG2aS1                             |LOPIT experiment on Mouse E14TG2a Embryonic Stem Cells from Breckels et al. (2016)                                             |
|E14TG2aS1goCC                         |LOPIT experiment on Mouse E14TG2a Embryonic Stem Cells from Breckels et al. (2016)                                             |
|E14TG2aS1yLoc                         |LOPIT experiment on Mouse E14TG2a Embryonic Stem Cells from Breckels et al. (2016)                                             |
|E14TG2aS2                             |LOPIT experiment on Mouse E14TG2a Embryonic Stem Cells from Breckels et al. (2016)                                             |
|HEK293T2011                           |LOPIT experiment on Human Embryonic Kidney fibroblast HEK293T cells from Breckels et al. (2013)                                |
|HEK293T2011goCC                       |LOPIT experiment on Human Embryonic Kidney fibroblast HEK293T cells from Breckels et al. (2013)                                |
|HEK293T2011hpa                        |LOPIT experiment on Human Embryonic Kidney fibroblast HEK293T cells from Breckels et al. (2013)                                |
|Kozik_con                             |Small molecule enhancers of endosome-to-cytosol import augment anti-tumour immunity                                            |
|Kozik_pra                             |Small molecule enhancers of endosome-to-cytosol import augment anti-tumour immunity                                            |
|Kozik_tam                             |Small molecule enhancers of endosome-to-cytosol import augment anti-tumour immunity                                            |
|Shin2019MitoControlrep1               |Spatial proteomics defines the content of trafficking vesicles captured by golgin tethers                                      |
|Shin2019MitoControlrep2               |Spatial proteomics defines the content of trafficking vesicles captured by golgin tethers                                      |
|Shin2019MitoControlrep3               |Spatial proteomics defines the content of trafficking vesicles captured by golgin tethers                                      |
|Shin2019MitoGcc88rep1                 |Spatial proteomics defines the content of trafficking vesicles captured by golgin tethers                                      |
|Shin2019MitoGcc88rep2                 |Spatial proteomics defines the content of trafficking vesicles captured by golgin tethers                                      |
|Shin2019MitoGcc88rep3                 |Spatial proteomics defines the content of trafficking vesicles captured by golgin tethers                                      |
|Shin2019MitoGol97rep1                 |Spatial proteomics defines the content of trafficking vesicles captured by golgin tethers                                      |
|Shin2019MitoGol97rep2                 |Spatial proteomics defines the content of trafficking vesicles captured by golgin tethers                                      |
|Shin2019MitoGol97rep3                 |Spatial proteomics defines the content of trafficking vesicles captured by golgin tethers                                      |
|andreyev2010                          |Six sub-cellular fraction data from mouse macrophage-like RAW264.7 cells from Andreyev et al. (2009)                           |
|andreyev2010activ                     |Six sub-cellular fraction data from mouse macrophage-like RAW264.7 cells from Andreyev et al. (2009)                           |
|andreyev2010rest                      |Six sub-cellular fraction data from mouse macrophage-like RAW264.7 cells from Andreyev et al. (2009)                           |
|andy2011                              |LOPIT experiment on Human Embryonic Kidney fibroblast HEK293T cells from Breckels et al. (2013)                                |
|andy2011goCC                          |LOPIT experiment on Human Embryonic Kidney fibroblast HEK293T cells from Breckels et al. (2013)                                |
|andy2011hpa                           |LOPIT experiment on Human Embryonic Kidney fibroblast HEK293T cells from Breckels et al. (2013)                                |
|at_chloro                             |The AT_CHLORO data base                                                                                                        |
|baers2018                             |Synechocystis spatial proteomics                                                                                               |
|beltran2016HCMV120                    |Data from Beltran et al. 2016                                                                                                  |
|beltran2016HCMV24                     |Data from Beltran et al. 2016                                                                                                  |
|beltran2016HCMV48                     |Data from Beltran et al. 2016                                                                                                  |
|beltran2016HCMV72                     |Data from Beltran et al. 2016                                                                                                  |
|beltran2016HCMV96                     |Data from Beltran et al. 2016                                                                                                  |
|beltran2016MOCK120                    |Data from Beltran et al. 2016                                                                                                  |
|beltran2016MOCK24                     |Data from Beltran et al. 2016                                                                                                  |
|beltran2016MOCK48                     |Data from Beltran et al. 2016                                                                                                  |
|beltran2016MOCK72                     |Data from Beltran et al. 2016                                                                                                  |
|beltran2016MOCK96                     |Data from Beltran et al. 2016                                                                                                  |
|courtland_control                     |Genetic Disruption of WASHC4 Drives Endo-lysosomal Dysfunction and Cognitive-Movement Impairments in Mice and Humans           |
|courtland_mutant                      |Genetic Disruption of WASHC4 Drives Endo-lysosomal Dysfunction and Cognitive-Movement Impairments in Mice and Humans           |
|davies2018ap4b1                       |AP-4 vesicles contribute to spatial control of autophagy via RUSC-dependent peripheral delivery of ATG9A                       |
|davies2018ap4e1                       |AP-4 vesicles contribute to spatial control of autophagy via RUSC-dependent peripheral delivery of ATG9A                       |
|davies2018wt                          |AP-4 vesicles contribute to spatial control of autophagy via RUSC-dependent peripheral delivery of ATG9A                       |
|dunkley2006                           |LOPIT data from Dunkley et al. (2006)                                                                                          |
|dunkley2006goCC                       |LOPIT data from Dunkley et al. (2006)                                                                                          |
|fabre2015r1                           |Data from Fabre et al. 2015                                                                                                    |
|fabre2015r2                           |Data from Fabre et al. 2015                                                                                                    |
|foster2006                            |PCP data from Foster et al. (2006)                                                                                             |
|groen2014cmb                          |LOPIT experiments on Arabidopsis thaliana roots, from Groen et al. (2014)                                                      |
|groen2014r1                           |LOPIT experiments on Arabidopsis thaliana roots, from Groen et al. (2014)                                                      |
|groen2014r1goCC                       |LOPIT experiments on Arabidopsis thaliana roots, from Groen et al. (2014)                                                      |
|groen2014r2                           |LOPIT experiments on Arabidopsis thaliana roots, from Groen et al. (2014)                                                      |
|groen2014r3                           |LOPIT experiments on Arabidopsis thaliana roots, from Groen et al. (2014)                                                      |
|hall2009                              |LOPIT data from Hall et al. (2009)                                                                                             |
|havugimana2012                        |Data from Havugimana et al. 2012                                                                                               |
|hirst2018                             |Data from Hirst et al. 2018                                                                                                    |
|hyperLOPIT2015                        |Protein and PMS-level hyperLOPIT datasets on Mouse E14TG2a embryonic stem cells from Christoforou et al. (2016).               |
|hyperLOPIT2015_se                     |Protein and PMS-level hyperLOPIT datasets on Mouse E14TG2a embryonic stem cells from Christoforou et al. (2016).               |
|hyperLOPIT2015goCC                    |Protein and PMS-level hyperLOPIT datasets on Mouse E14TG2a embryonic stem cells from Christoforou et al. (2016).               |
|hyperLOPIT2015ms2                     |Protein and PMS-level hyperLOPIT datasets on Mouse E14TG2a embryonic stem cells from Christoforou et al. (2016).               |
|hyperLOPIT2015ms2psm                  |Protein and PMS-level hyperLOPIT datasets on Mouse E14TG2a embryonic stem cells from Christoforou et al. (2016).               |
|hyperLOPIT2015ms3r1                   |Protein and PMS-level hyperLOPIT datasets on Mouse E14TG2a embryonic stem cells from Christoforou et al. (2016).               |
|hyperLOPIT2015ms3r1psm                |Protein and PMS-level hyperLOPIT datasets on Mouse E14TG2a embryonic stem cells from Christoforou et al. (2016).               |
|hyperLOPIT2015ms3r2                   |Protein and PMS-level hyperLOPIT datasets on Mouse E14TG2a embryonic stem cells from Christoforou et al. (2016).               |
|hyperLOPIT2015ms3r2psm                |Protein and PMS-level hyperLOPIT datasets on Mouse E14TG2a embryonic stem cells from Christoforou et al. (2016).               |
|hyperLOPIT2015ms3r3                   |Protein and PMS-level hyperLOPIT datasets on Mouse E14TG2a embryonic stem cells from Christoforou et al. (2016).               |
|hyperLOPITU2OS2017                    |2017 and 2018 hyperLOPIT on U2OS cells                                                                                         |
|hyperLOPITU2OS2017b                   |2017 and 2018 hyperLOPIT on U2OS cells                                                                                         |
|hyperLOPITU2OS2018                    |2017 and 2018 hyperLOPIT on U2OS cells                                                                                         |
|itzhak2016helaCtrl                    |Global, quantitative and dynamic mapping of protein subcellular localization                                                   |
|itzhak2016helaEgf                     |Global, quantitative and dynamic mapping of protein subcellular localization                                                   |
|itzhak2016stcSILAC                    |                                                                                                                               |
|itzhak2017                            |Data from Itzhak et al. 2017                                                                                                   |
|itzhak2017markers                     |Data from Itzhak et al. 2017                                                                                                   |
|kirkwood2013                          |Data from Kirkwood et al. 2013.                                                                                                |
|krahmer2018pcp                        |Subcellular Reorganization in Diet-Induced Hepatic Steatosis                                                                   |
|krahmer2018phosphopcp                 |Subcellular Reorganization in Diet-Induced Hepatic Steatosis                                                                   |
|kristensen2012r1                      |Data from Kristensen et al. 2012                                                                                               |
|kristensen2012r2                      |Data from Kristensen et al. 2012                                                                                               |
|kristensen2012r3                      |Data from Kristensen et al. 2012                                                                                               |
|lopimsSyn1                            |LOPIMS data for the Synapter 2.0 paper                                                                                         |
|lopimsSyn2                            |LOPIMS data for the Synapter 2.0 paper                                                                                         |
|lopimsSyn2_0frags                     |LOPIMS data for the Synapter 2.0 paper                                                                                         |
|lopitdcU2OS2018                       |2017 and 2018 hyperLOPIT on U2OS cells                                                                                         |
|lpsTimecourse_mulvey2021              |Protein and PMS-level datasets from temporal abundance profiling experiments of THP-1 human leukaema cells stimulated with LPS |
|lpsTimecourse_rep1_mulvey2021         |Protein and PMS-level datasets from temporal abundance profiling experiments of THP-1 human leukaema cells stimulated with LPS |
|lpsTimecourse_rep2_mulvey2021         |Protein and PMS-level datasets from temporal abundance profiling experiments of THP-1 human leukaema cells stimulated with LPS |
|lpsTimecourse_rep3_mulvey2021         |Protein and PMS-level datasets from temporal abundance profiling experiments of THP-1 human leukaema cells stimulated with LPS |
|moloneyTbBSF                          |Spatial proteomics datasets from two African trypanosome species                                                               |
|moloneyTbPCF                          |Spatial proteomics datasets from two African trypanosome species                                                               |
|moloneyTcBSF                          |Spatial proteomics datasets from two African trypanosome species                                                               |
|moloneyTcPCF                          |Spatial proteomics datasets from two African trypanosome species                                                               |
|mulvey2015                            |Data from Mulvey et al. 2015                                                                                                   |
|mulvey2015_se                         |Data from Mulvey et al. 2015                                                                                                   |
|mulvey2015norm                        |Data from Mulvey et al. 2015                                                                                                   |
|mulvey2015norm_se                     |Data from Mulvey et al. 2015                                                                                                   |
|nikolovski2012                        |Meta-analysis from Nikolovski et al. (2012)                                                                                    |
|nikolovski2012imp                     |Meta-analysis from Nikolovski et al. (2012)                                                                                    |
|nikolovski2014                        |LOPIMS data from Nikolovski et al. (2014)                                                                                      |
|orre2019a431                          |SubCellBarCode: Proteome-wide Mapping of Protein Localization and Relocalization                                               |
|orre2019h322                          |SubCellBarCode: Proteome-wide Mapping of Protein Localization and Relocalization                                               |
|orre2019hcc827                        |SubCellBarCode: Proteome-wide Mapping of Protein Localization and Relocalization                                               |
|orre2019hcc827gef                     |SubCellBarCode: Proteome-wide Mapping of Protein Localization and Relocalization                                               |
|orre2019hcc827rep1                    |SubCellBarCode: Proteome-wide Mapping of Protein Localization and Relocalization                                               |
|orre2019hcc827rep2                    |SubCellBarCode: Proteome-wide Mapping of Protein Localization and Relocalization                                               |
|orre2019hcc827rep3                    |SubCellBarCode: Proteome-wide Mapping of Protein Localization and Relocalization                                               |
|orre2019mcf7                          |SubCellBarCode: Proteome-wide Mapping of Protein Localization and Relocalization                                               |
|orre2019u251                          |SubCellBarCode: Proteome-wide Mapping of Protein Localization and Relocalization                                               |
|psms_lpsTimecourse_rep1_mulvey2021    |Protein and PMS-level datasets from temporal abundance profiling experiments of THP-1 human leukaema cells stimulated with LPS |
|psms_lpsTimecourse_rep2_mulvey2021    |Protein and PMS-level datasets from temporal abundance profiling experiments of THP-1 human leukaema cells stimulated with LPS |
|psms_lpsTimecourse_rep3_mulvey2021    |Protein and PMS-level datasets from temporal abundance profiling experiments of THP-1 human leukaema cells stimulated with LPS |
|psms_thpLOPIT_lps_rep1_set1           |Protein and PMS-level hyperLOPIT datasets from THP-1 human leukaema cells                                                      |
|psms_thpLOPIT_lps_rep1_set2           |Protein and PMS-level hyperLOPIT datasets from THP-1 human leukaema cells                                                      |
|psms_thpLOPIT_lps_rep2_set1           |Protein and PMS-level hyperLOPIT datasets from THP-1 human leukaema cells                                                      |
|psms_thpLOPIT_lps_rep2_set2           |Protein and PMS-level hyperLOPIT datasets from THP-1 human leukaema cells                                                      |
|psms_thpLOPIT_lps_rep3_set1           |Protein and PMS-level hyperLOPIT datasets from THP-1 human leukaema cells                                                      |
|psms_thpLOPIT_lps_rep3_set2           |Protein and PMS-level hyperLOPIT datasets from THP-1 human leukaema cells                                                      |
|psms_thpLOPIT_unstim_rep1_set1        |Protein and PMS-level hyperLOPIT datasets from THP-1 human leukaema cells                                                      |
|psms_thpLOPIT_unstim_rep1_set2        |Protein and PMS-level hyperLOPIT datasets from THP-1 human leukaema cells                                                      |
|psms_thpLOPIT_unstim_rep2_set1        |Protein and PMS-level hyperLOPIT datasets from THP-1 human leukaema cells                                                      |
|psms_thpLOPIT_unstim_rep2_set2        |Protein and PMS-level hyperLOPIT datasets from THP-1 human leukaema cells                                                      |
|psms_thpLOPIT_unstim_rep3_set1        |Protein and PMS-level hyperLOPIT datasets from THP-1 human leukaema cells                                                      |
|psms_thpLOPIT_unstim_rep3_set2        |Protein and PMS-level hyperLOPIT datasets from THP-1 human leukaema cells                                                      |
|rodriguez2012r1                       |Spatial proteomics of human inducible goblet-like LS174T cells from Rodriguez-Pineiro et al. (2012)                            |
|rodriguez2012r2                       |Spatial proteomics of human inducible goblet-like LS174T cells from Rodriguez-Pineiro et al. (2012)                            |
|rodriguez2012r3                       |Spatial proteomics of human inducible goblet-like LS174T cells from Rodriguez-Pineiro et al. (2012)                            |
|stekhoven2014                         |Data from Stekhoven et al. 2014                                                                                                |
|tan2009r1                             |LOPIT data from Tan et al. (2009)                                                                                              |
|tan2009r1goCC                         |LOPIT data from Tan et al. (2009)                                                                                              |
|tan2009r2                             |LOPIT data from Tan et al. (2009)                                                                                              |
|tan2009r3                             |LOPIT data from Tan et al. (2009)                                                                                              |
|thpLOPIT_lps_mulvey2021               |Protein and PMS-level hyperLOPIT datasets from THP-1 human leukaema cells                                                      |
|thpLOPIT_lps_rep1_mulvey2021          |Protein and PMS-level hyperLOPIT datasets from THP-1 human leukaema cells                                                      |
|thpLOPIT_lps_rep2_mulvey2021          |Protein and PMS-level hyperLOPIT datasets from THP-1 human leukaema cells                                                      |
|thpLOPIT_lps_rep3_mulvey2021          |Protein and PMS-level hyperLOPIT datasets from THP-1 human leukaema cells                                                      |
|thpLOPIT_unstimulated_mulvey2021      |Protein and PMS-level hyperLOPIT datasets from THP-1 human leukaema cells                                                      |
|thpLOPIT_unstimulated_rep1_mulvey2021 |Protein and PMS-level hyperLOPIT datasets from THP-1 human leukaema cells                                                      |
|thpLOPIT_unstimulated_rep2_mulvey2021 |Protein and PMS-level hyperLOPIT datasets from THP-1 human leukaema cells                                                      |
|thpLOPIT_unstimulated_rep3_mulvey2021 |Protein and PMS-level hyperLOPIT datasets from THP-1 human leukaema cells                                                      |
|trotter2010                           |LOPIT data sets used in Trotter et al. (2010)                                                                                  |
|trotter2010shallow                    |LOPIT data sets used in Trotter et al. (2010)                                                                                  |
|trotter2010steep                      |LOPIT data sets used in Trotter et al. (2010)                                                                                  |
|yeast2018                             |Saccharomyces cerevisiae spatial proteomics (2018)                                                                             |

### Loading data

Data is loaded into the `R` session using the `load` function; for
instance, to get the data from
[Dunkley et al (2006)](http://www.pnas.org/content/103/17/6518.abstract),
one would type


```r
data(dunkley2006)
```

To get more information about a given dataset, see its manual page


```r
?dunkley2006
## or
help("dunkley2006")
```

## The datasets

Each data object in `pRolocdata` is available as an `MSnSet`
instance. The instances contain the actual quantitative data, sample
and features annotations (see `pData` and `fData`
respectively). Additional MIAPE data
[[1](https://en.wikipedia.org/wiki/Minimum_Information_About_a_Proteomics_Experiment),
[2](http://www.nature.com/nbt/journal/v25/n8/abs/nbt1329.html)]
experimental data is available in the `experimentData` slot, as
described in section *Required metadata* below.

The source of these data is generally one or several text-based
spreadsheet (`csv`, `tsv`) produced by a third-party
application. These original files are often distributed as
supplementary material to the research paper and used to generate the
`R` objects. These source spreadsheets are available in the package's
`inst/extdata` directory. The `R` script files, that read the
spreadsheets and create the `R` data is distributed in the
`inst/scripts` directory.

### Suggested metadata

Additional metadata is available with the `pRolocmetadata()` function
as detailed below.

#### Species
Documented in `experimentData(.)@samples$species`

#### Tissue

Documented in `experimentData(.)@samples$tissue`. If tissue is `Cell`,
then details about the cell line are available in
`experimentData(.)@samples$cellLine`.

#### PMID
Documented in `pubMedIds(.)`.

#### Spatial proteomics experiment annotation

Documented in `experimentData(.)@other`:
  - **MS** (`$MS`) type of mass spectrometry experiment: iTRAQ8,
	iTRAQ4, TMT6, LF, SC, ...
  - **Experiment** (`$spatexp`) type of spatial proteomics
	experiment: LOPIT, LOPIMS, subtractive, PCP, other, PCP-SILAC,
	...
  - **MarkerCol** (`$markers.fcol`) name of the markers feature
	data. Default is `markers`.
  - **PredictionCol** (`$prediction.fcol`) name of the localisation
	prediction feature data.

#### Example


```r
experimentData(dunkley2006)@samples
```

```
## $species
## [1] "Arabidopsis thaliana"
## 
## $tissue
## [1] "Callus"
```

```r
pubMedIds(dunkley2006)
```

```
## [1] "16618929"
```

```r
otherInfo(experimentData(dunkley2006))
```

```
## $MS
## [1] "iTRAQ4"
## 
## $spatexp
## [1] "LOPIT"
## 
## $markers.fcol
## [1] "pd.markers"
## 
## $prediction.fcol
## [1] "pd.2013"
```

```r
## all at once
pRolocmetadata(dunkley2006)
```

```
## pRoloc experiment metadata:
##  Species: Arabidopsis thaliana
##  Tissue: Callus
##  CellLine: NA
##  PMID: 16618929
##  MS: iTRAQ4
##  Experiment: LOPIT
##  MarkerCol: pd.markers
##  PredictionCol: pd.2013
```

### Adding new data

The procedure to data in pRolocdata is as follows. Here, we assume
that 3 new data files are available from the manuscript of *Smith et
al. 2017*, and these files will be added to `pRolocdata` as three
`MSnSet` objects.


1. the original data (often from supplementary material) are added to
   `inst/extdata`, say `Smith_expA.csv`, `Smith_expB.csv` and
   `Smith_expC.csv` (the name should ideally be the same as the
   original files), and the files and provenance is documented in
   `inst/extdata/README`. If the data files are really big, then they
   should be compressed. If they are too big (for example don't fit on
   github or would substantially increase the size of the package),
   then we might decide not to added them, but they should still be
   documented in the README file and the script (see point 2) should
   still assume they are there.

2. A script, typically called `Smith2017.R`, is added to
   `inst/scripts/`. That script reads the files above and saves the
   corresponding (compressed) MSnSet objects directly in data,
   typically called `Smith2016a.rda`, `Smith2016a.rda`, ..., and the
   objects themselves would be named `Smith2016a`, `Smith2016b`, ...

3. Write a `man/Smith2016.Rd` documentation file documenting all
   relevant data objects, providing some information about the
   experiment and data provenance, and a reference to the original
   paper.

4. Build and check the package and, if successful, send a [github pull
   request](https://github.com/lgatto/pRolocdata).


If you do not have the `R` expertise to prepare the data, please
[open an issue](https://github.com/lgatto/pRolocdata/issues) in the 
`pRolocdata` Github repo or send me an email at 
`laurent.gatto<AT>uclouvain<dot>be` with the source `csv`
files and appropriate metadata and I will add it for you.
