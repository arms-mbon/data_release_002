### data_release_002

These are the second set of data files to be submitted to (Eur)OBIS: taxonomic occurrences from the COI, 18S, and ITS marker gene omics data, sampling event metadata, and image metadata for the events of ARMS-MBON's second sampling campaign (all ARMS deployed in 2020 and 2021 and retrieved between and 2020 and 2022). This includes: 

* The individual files that when combined, create the DwCA files that we submitted: a file of occurrences (taxonomy and event data), the DNA extension information (omics data), the EMOF (extra information that cannot otherwise be added to the other two files).
* The observatory, sampling event, omics and image data related to the sampling events included in this EurOBIS dataset. These expand somewhat on the information included in the data that will be published in (Eur)OBIS.

The source files for the omics and taxonomic data can be found in [the analysis_release_002](https://github.com/arms-mbon/analysis_release_002) repository: the input and output files for the bioinformatics analysis done with PEMA can be found there. Links to the PEMA pipeline can also be found there. The code that was used to reforumlate PEMA outputs and search various databases for associated information can be found in [code_release_002](https://github.com/arms-mbon/code_release_002). 

Contaminants have been filtered out with **decontam** (R) using run-specific negative controls and the prevalence method. ASVs flagged as contaminants were removed prior to data release. Detailed scripts are provided in [code_release_002](https://github.com/arms-mbon/code_release_002).

For more information on ARMS-MBON, see its [data landing page](https://data.arms-mbon.org/) and references there in. 

  
## The sampling event data
These are the files that contain the sampling event data. This is a subset of the entire ARMS-MBON set of [combined event data](https://github.com/arms-mbon/data_workspace/tree/main/qualitycontrolled_data/combined), and include: 
* A CSV data file containing [observatory metadata](https://github.com/arms-mbon/data_release_002/blob/main/ObservatoryData_release002.csv), with an accompanying metadata file
* A CSV data file containing [sampling event metadata](https://github.com/arms-mbon/data_release_002/blob/main/SamplingEventData_release002.csv), with an accompanying metadata file
* A CSV data file containing [raw sequence metadata](https://github.com/arms-mbon/data_release_002/blob/main/OmicsData_release002.csv), with an accompanying metadata file; including the ENA accession numbers and a limited amount of additional omics metadata. For more information on the processing of the samples and subsequence bioinformatics, see the [analysis_release_002](https://github.com/arms-mbon/analysis_release_002) repository.
* A CSV data file containing [images metadata](https://github.com/arms-mbon/data_release_002/blob/main/ImageData_release002.csv), with an accompanying metadata file (note that there are 1000s of rows in this spreadsheet), with a metadata file that explains the entries therein. Images are currently stored in PlutoF and can be downloaded by accessing the links in the "Download URL" column.

Note that these files [in the combined data folder](https://github.com/arms-mbon/data_workspace/tree/main/qualitycontrolled_data/combined) may also be useful to you:
*  A [list of the ENA project, sample, and run accession numbers](https://github.com/arms-mbon/data_workspace/blob/main/qualitycontrolled_data/combined/ena_accession_numbers.xlsx) for all the ARMS-MBON data to date
*  A [list of the area/field and sample/technical replicates](https://github.com/arms-mbon/data_workspace/blob/main/qualitycontrolled_data/combined/replicates_list.csv) for all the ARMS-MBON data to date
*  Additional sequencing demultiplexing metadata - see the README in the folder for an explanation; the subset of those samples relevant to this data release can be found on [demultiplexing_details_OmicsData_release002.csv](https://github.com/arms-mbon/data_release_002/blob/main/demultiplexing_details_OmicsData_release002.csv). 


