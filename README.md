# Data constructed for Drug repurposing
---

Data used for model building was obtained from creditable sources. 
For drugs, the main inclusion criterion was FDA approval. The InChI values were obtained from a comprehensive and popular source, the DrugBank.
For viruses, the main inclusion criterion was based on the FDA-approved antiviral-drug list from the Virus Pathogen Resource (ViPR). 

## Description of the Data and file structure

Drugs and viruses were mapped with information from the NCBI Viral Genomes Resource. The genome sequences were retrieved from the GenBank, which documents RNA viruses in DNA format. The unique number of genome sequences at the nucleotide level in FASTA representation was 1353. 

Data for the analysis was constructed in a way suitable for the classification setup.

The constructed dataset based on the above descriptions are the FOUR columns: 
"d_name" – the role of data in the model
"DrugBank_Id" – the DrugBankID of the InChi representation to be input
"Raw_FASTA" – the whole genome sequence of the virus in DNA form 
"y_true" – the actual condition of the match

The additional TWO columns are from processing with a deep learning model:
"y_pred" – the predicted condition of the match
"y_score" – the predicted score by a model


## Sharing/access Information
GenBank: https://ftp.ncbi.nlm.nih.gov/genbank/
NCBI Viral Genomes Resource: https://www.ncbi.nlm.nih.gov/genome/viruses/
DrugBank: https://go.drugbank.com/releases/latest 

