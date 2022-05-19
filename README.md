# Ocean Sampling Day 2014 space

These are the files for Ocean Sampling Day 2014. These data are published in PANGEA (https://doi.pangaea.de/10.1594/PANGAEA.854419) and are the first OSD published dataset. The OSD project was taken up again in 2018 by ASSEMBLE Plus and those 2018 onwards data are published via the IMIS metadata catalogue. To provide consistency between the 2014 and these subsequence 2018+ records, a record for the OSD2014 even was also created in IMIS (http://www.assembleplus.eu/information-system?module=dataset&dasid=8044).<br>
The data for the OSD2014 event should be taken from PANGEA. However, as it was decided to publish the OSD2018+ data in machine-accessible formats and with semantic annotation, we decided to do the same for the 2014 data. Hence, the PANGEA dataset has been so annotated and reformated and these data are provided here in Github. Note that in this process -- and in particular to provide consistency with the OSD2018+ data -- some of the column names from the PANGEA dataset have been changed and the formatting of the sample IDs also: see the two mapping files provided here to learn more. <br>

The documentation added here includes:

* [The OSD Handbook](https://github.com/ocean-sampling-day/ToPublish/blob/main/IMIS/OSD2014/OSD_Handbook_2014-06.pdf)
* The two sampling protocols that were used:
    - [OSD2014_protocol_A](https://github.com/ocean-sampling-day/ToPublish/blob/main/IMIS/OSD2014/OSD2014_protocol_A_sterivex_filtration_methods.pdf)
    - [OSD2014_protocol_B](https://github.com/ocean-sampling-day/ToPublish/blob/main/IMIS/OSD2014/OSD2014_protocol_B_18S_V4andV9_Sequencing_LifeWath_MoBiLab_BARI.pdf)

The data files provided are:

* A CSV Data file with the collected environmental, event, and omics data: [OSD14Data_version1.csv](https://github.com/ocean-sampling-day/ToPublish/blob/main/IMIS/OSD2014/OSD14Data_version1.csv)   
The omics data are the ENA BioSample and Sample accession numbers for the sequences that are associated with each sample. 
* For those accessing these data programmatically: a .ttl (turtle) files describe the data file for machines; which was generated based on the .ldt (linked data template).
* Two Metadata files in which the columns titles and units used in the Data file are semantically annotated and explained:
    - [OSD14Metadata_HumanReadable_version1.csv](https://github.com/ocean-sampling-day/ToPublish/blob/main/IMIS/OSD2014/OSD14Metadata_HumanReadable_version1.csv)
    - [OSD14Metadata_MachineReadable_version1.csv](https://github.com/ocean-sampling-day/ToPublish/blob/main/IMIS/OSD2014/OSD14Metadata_MachineReadable_version1.csv) - which is necessary to generate the turtle file. 
* Two metadata mapping files in which the differences between the PANGEA format and our IMIS format are outlined: 
  - [OSD14Metadata_Pangea2IMIS_columns.csv](https://github.com/ocean-sampling-day/ToPublish/blob/main/IMIS/OSD2014/OSD14Metadata_Pangea2IMIS_columns.csv) shows the relationship between the column titles as used in these two catalogues, 
  - [OSD14_Metadata_Pangea2IMIS_values.csv](https://github.com/ocean-sampling-day/ToPublish/blob/main/IMIS/OSD2014/OSD14_Metadata_Pangea2IMIS_values.csv) shows the formatted we used in IMIS for the event and sample IDs compared to those used in PANGEA
* A list of the details of the OSD stations [OSDStations.csv](https://github.com/ocean-sampling-day/ToPublish/blob/main/IMIS/OSD2014/OSDStations.csv)
* A CSV file containing the ENA Sample and Run accession numbers, the sample title (aka SampleID), and the target gene (being 16S, 18S, or MG=metagenomics) is provided here as [OSD2014_AccessionNumbers.csv](https://raw.githubusercontent.com/ocean-sampling-day/OSD2014/main/OSD2014_AccessionNumbers.csv).


As of April 2022 we noticed that some accession numbers were not accessible in ENA:
  1. Eight accession numbers in our CSV data file are not present in ENA and do not have any associated ENA information (more specifically: SAMEA3275501, SAMEA3275510, SAMEA3275511, SAMEA3275513, SAMEA3275528, SAMEA3275566, SAMEA3275569, SAMEA3275587, SAMEA3275606, SAMEA3275613, SAMEA3275644).
  2. Two accession numbers in ENA were missing from our CSV data file (more specifically: SAMEA3282990, SAMEA3340641). These have now been added to the CSV data file.
  
Note that scans of the logsheets can be found in the PANGEA record. 

Also provided via this OSD Github space are the OSD2019 (https://github.com/ocean-sampling-day/ToPublish/tree/main/IMIS/OSD2019) and OSD2018 data (https://github.com/ocean-sampling-day/ToPublish/tree/main/IMIS/OSD2018).
