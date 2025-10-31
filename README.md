# data_release_002

<!--
* OBIS dataset [ITS](https://obis.org/dataset/...), and its [metadata record](https://doi.org/10.14284/...)
 -->

**UPDATES** <br>
These data are now available via MarineInfo. They will appear in EurOBIS shortly.
* 18S dataset [metadata record](https://www.vliz.be/en/imis?module=dataset&dasid=8918)
* ITS dataset [metadata record](https://www.vliz.be/en/imis?module=dataset&dasid=8921)
* COI dataset [metadata record](https://www.vliz.be/en/imis?module=dataset&dasid=8922)

These are the second set of data files released from the ARMS-MBON project: taxonomic occurrences from the COI, 18S, and ITS marker gene omics data, sampling event metadata, and image metadata for the events of ARMS-MBON's second sampling campaign (all ARMS deployed in 2020 and 2021 and retrieved between and 2020 and 2022). These data have been published in the IMIS catalogue, which is part of MarineInfo, and are in the process of being intested into EurOBIS. Once the data are in EurOBIS (and from there, harvested into OBIS and GBIF), the respective links will appear in the metadata records given in the links above. 

This datasets is also available from here. The data here are: 

* The three 18S files: [DNA extension](https://github.com/arms-mbon/data_release_002/blob/main/ARMS_18S_DNAextension.csv), [EMOF](https://github.com/arms-mbon/data_release_002/blob/main/ARMS_18S_EMOF.csv), [Occurrence extension](https://github.com/arms-mbon/data_release_002/blob/main/ARMS_18S_Occurrence.csv) (processed dates: April 2021, Aug. 2023, Sept 2020)
* The three CO1 files: [DNA extension](https://github.com/arms-mbon/data_release_002/blob/main/ARMS_COI_DNAextension.csv), [EMOF](https://github.com/arms-mbon/data_release_002/blob/main/ARMS_COI_EMOF.csv), [Occurrence extension](https://github.com/arms-mbon/data_release_002/blob/main/ARMS_COI_Occurrence.csv) (processed dates: April 2021, Aug. 2023, Sept 2020)
* The three ITS files: [DNA extension](https://github.com/arms-mbon/data_release_002/blob/main/ARMS_ITS_DNAextension.csv), [EMOF](https://github.com/arms-mbon/data_release_002/blob/main/ARMS_ITS_EMOF.csv), [Occurrence extension](https://github.com/arms-mbon/data_release_002/blob/main/ARMS_ITS_Occurrence.csv) (processed dates: April 2021, Sept. 2020)
* The [observatory data](https://github.com/arms-mbon/data_release_002/blob/main/ObservatoryData_release002.csv) and a metadata file explaining the entries therein; [sampling event data](https://github.com/arms-mbon/data_release_002/blob/main/SamplingEventData_release002.csv) (and its metadata file), [omics data](https://github.com/arms-mbon/data_release_002/blob/main/OmicsData_release002.csv) (and its metadata file). These are subset of the entire ARMS-MBON data set that can be found in [combined event data](https://github.com/arms-mbon/data_workspace/tree/main/qualitycontrolled_data/combined)
* Additionally, a file with metadata about the [images](https://github.com/arms-mbon/data_release_002/blob/main/ImageData_release002.csv) obtained during the sampling events and of the ARMS plates. These are subset of the entire ARMS-MBON data set that can be found in [combined event data](https://github.com/arms-mbon/data_workspace/tree/main/qualitycontrolled_data/combined). Images are currently stored in PlutoF and can be downloaded by accessing the links in the "Download URL" column. 

The source files for the omics and taxonomic data can be found in [the analysis_release_002](https://github.com/arms-mbon/analysis_release_002) repository: the input and output files for the bioinformatics analysis done with PEMA can be found there. Links to the PEMA pipeline can also be found there. The code that was used to reforumlate PEMA outputs and search various databases for associated information can be found in [code_release_002](https://github.com/arms-mbon/code_release_002). These essentially tidy up the taxonomic names to be more suitable for including in a biodiversity (as opposed to a genomics) database. The DwC generator code then applies some additional tidying up, to conform to what EurOBIS in particular require, as is explained in the [DwC generator repository](https://github.com/arms-mbon/darwin-core-generator/tree/v2.0.0)

The code that turned the data into DwC can be found in [DwC generator](https://github.com/arms-mbon/darwin-core-generator). This code is being used for all the ARMS-MBON data released, and the version that was used specifically for this data release 002 can be found in the tagged repository [v2.0.0][(https://github.com/arms-mbon/darwin-core-generator/tree/v2.0.0). 

Contaminants have been filtered out with **decontam** (R) using run-specific negative controls and the prevalence method. ASVs flagged as contaminants were removed prior to data release. Detailed scripts are provided in [code_release_002](https://github.com/arms-mbon/code_release_002).

For more information on ARMS-MBON, see its [data landing page](https://data.arms-mbon.org/) and references there in. 

Note that these files [in the combined data folder](https://github.com/arms-mbon/data_workspace/tree/main/qualitycontrolled_data/combined) may also be useful to you:
*  A [list of the ENA project, sample, and run accession numbers](https://github.com/arms-mbon/data_workspace/blob/main/qualitycontrolled_data/combined/ena_accession_numbers.xlsx) for all the ARMS-MBON data to date
*  A [list of the area/field and sample/technical replicates](https://github.com/arms-mbon/data_workspace/blob/main/qualitycontrolled_data/combined/replicates_list.csv) for all the ARMS-MBON data to date
*  Additional sequencing demultiplexing metadata - see the README in the folder for an explanation; the subset of those samples relevant to this data release can be found on [demultiplexing_details_OmicsData_release002.csv](https://github.com/arms-mbon/data_release_002/blob/main/demultiplexing_details_OmicsData_release002.csv). 


