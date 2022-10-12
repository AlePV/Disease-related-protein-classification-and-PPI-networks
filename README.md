# Welcome to the Ramirez Lab Wiki - Knime: Disease related protein classification and PPI networks #

This Knime workflow uses multiple databases to search for disease related proteins by experimental reports or manual annotations, then proteins are classified by the development phase of their related drugs and a protein-protein network is generated.

<p align="center">
    <img src="https://github.com/AlePV/Disease_related_protein_classification_and_PPI_networks/blob/main/media/Disease_related_protein_classification_and_PPI_networks_WF.png?raw=true" width="1000">
</p>

## Requirements ##
- MySQL database service. [MySQL website and manual](https://dev.mysql.com/doc/refman/8.0/en/installing.html).
- Last ChEMBL MySQL database. [ChEBML databases](https://ftp.ebi.ac.uk/pub/databases/chembl/ChEMBLdb/latest/).
- "Target to disease mapping with ICD identifiers" and "Drug to disease mapping with ICD identifiers" files from TTD. [TTD full data downloads](http://db.idrblab.net/ttd/full-data-download). 
- Associated targets for a disease of choice on TSV format from Open Targets Platform. [Open Target Platform website](https://platform.opentargets.org/).
- Knime Analytics platform version 4.6.3 or higher. [Download Knime](https://www.knime.com/knime-analytics-platform).
- Our *in-house* [Knime](https://www.knime.com/) workflow [Disease_related_protein_classification_and_PPI_networks](https://github.com/ramirezlab/WIKI/raw/master/KNIME/Active%20compounds%20for%20a%20given%20target%20from%20ChEMBL/01_Active_compounds_for_a_given_target_from_ChEMBL.knwf).


**To follow these instructions you must have already installed [Knime](https://www.knime.com/), [MySQL](https://dev.mysql.com/doc/refman/8.0/en/installing.html) and configured the lastest [ChEBML database](https://ftp.ebi.ac.uk/pub/databases/chembl/ChEMBLdb/latest/) on your machine.**

## 1. Conect ChEMBL local MySQL database with the workflow ##

First download and import our workflow [Disease_related_protein_classification_and_PPI_networks](https://github.com/ramirezlab/WIKI/raw/master/KNIME/Active%20compounds%20for%20a%20given%20target%20from%20ChEMBL/01_Active_compounds_for_a_given_target_from_ChEMBL.knwf) to Knime software. Then configure **MySQL Connector** node by right clicking at the node and click configure, and complete Hostname, Database name, username and Password based on your personal MySQL information.

<p align="center">
<img src="https://github.com/AlePV/Disease_related_protein_classification_and_PPI_networks/blob/main/media/MySQL_Connector.png?raw=true" width="500">
</p>
