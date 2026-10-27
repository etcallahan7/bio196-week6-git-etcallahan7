RNA-seq sample metadata QC workflow by Ella Callahan
This repository demonstrates a small RNA-seq sample metadata quality-control workflow
- Within this repository there are directories data and scripts. Inside data is an example metadata.csv. It's a table giving iving the list of sample IDs and their associated condition, and replicate number. Inside scripts is a short script for reading such a metadata file. It ensures all the required columns are there (sample ID, condition, replicates) and breaks if there are any duplicate sample IDs. Then it tallies up the number of samples in each condition.
- To run qc workflow give the command Rscript scripts/qc_check.R from the repository root.
- After the script runs and checks the sample identifiers, the expected output is the number of samples in each condition. 
- Data policy: raw sequencing data, private data, credentials, and large generated files must not be committed
