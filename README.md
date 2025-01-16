#   NGS Data Analysis and Statistical Evaluation

# Overview
This project consists of two challenges focused on Data Handling and Statistical Analysis and NGS Data Analysis. The goal is to evaluate and analyze complex data related to phased methylation patterns (PMPs) and raw sequencing data from normal and cancer tissue samples. The tasks involve performing statistical analysis, alignment, mutation calling, and handling genomic data.

# Challenge 1: Data Handling and Statistical Analysis
  - Coverage Analysis: Calculate statistics like the median and coefficient of variation (CV) for single CpG coverage and generate plots to summarize coverage data.
  - Biomarker Identification: Identify PMPs that show high specificity for differentiating tissues and calculate the mean variant read fraction (VRF) for each PMP.
  - Addressing Specific Questions: Analyze the effect of sequencing depth on specificity, estimate the required read threshold for confident tissue classification, and compare the specificity of top 10 PMPs with individual CpG sites.

# Challenge 2: NGS Data Analysis
  - Quality Control: Perform quality control on FASTQ files using FastQC, summarize quality metrics.
  - Alignment and Mutation Calling: Align sequencing data to the human genome, perform somatic mutation detection, and identify mutations unique to cancer tissue.
  - Custom Code Development: Develop scripts using Samtools, bcftools, or Python/R to perform mutation detection and calculate necessary metrics.

# Install required Linux tools
  ~ apt-get install -y fastqc bowtie2 bwa samtools bcftools

# Install Python libraries
  ~ pip install matplotlib pysam pandas scikit-learn

# Dataset
  - The dataset consists of the following files: CpG Methylation Data: PupilBioTest_PMP_revA.csv – Contains methylation patterns across tissues.
  - NGS Data: FASTQ files for tumor and normal tissue samples in .fastq.gz format.
  - The files are expected to be provided via a secure link or uploaded to your environment.

# Running the Analysis
1. Data Handling and Statistical Analysis
    - Step 1: Coverage Analysis - This step calculates the median and coefficient of variation (CV) for single CpG coverage in each tissue. It also generates plots summarizing coverage statistics.
    - Step 2: Biomarker Identification - This part of the analysis uses statistical or machine learning approaches to identify PMPs that are highly specific for tissue differentiation. It also calculates the mean variant read fraction (VRF).

3. NGS Data Analysis
    - Step 1: Quality control on the raw sequencing data is performed using FastQC, and a summary of quality metrics is generated.
    - Step 2: Align the NGS data to the human genome and perform mutation calling using BWA, Mutect2, or a custom Python script.
    - Step 3: Using the normal tissue data, calculate the median background mutation level and determine the required reads per million for confident mutation calling.

# File Structure 
The project directory is structured as follows:

-  NGS_Data_Analysis_Task/
  -  scripts
  - data_handling_analysis.py (Code for coverage analysis and statistics)
  - biomarker_identification.py (Code for PMP identification and VRF calculation)
  - ngs_quality_control.py (Code for FastQC analysis)
  - ngs_mutation_detection.py (Code for mutation calling and analysis)
  - mutation_background_analysis.py (Code for background mutation calculation)
    
- Data/
  - PupilBioTest_PMP_revA.csv (Phased methylation patterns dataset)
  - NGS FASTQ files (Raw sequencing files)

- Results/
  - Generated plots (e.g., boxplots, bar charts)
  - Generated reports (e.g., summary of analysis)

- README.md (Project description and setup instructions)

# Notes for Reproducibility
  - Data Preprocessing: Ensure that all raw data (FASTQ files) and metadata (CSV files) are properly uploaded and linked in the code.
  - Dependencies: If any tool or library is not found in your system, please install them as specified above.
  - Parameter Files: Make sure to update file paths in the code with the correct file locations.

# Results
Upon running the scripts, the following results will be generated:
  - Coverage Analysis: Box plots summarizing the distribution of CpG coverage across tissues.
  - Biomarker Identification: A list of PMPs with their specificity and confidence metrics.
  - Mutation Analysis: Mutation distribution across chromosomes and background mutation levels.
  - Reports: Summary reports (in the results/reports/ folder) that detail the findings from the analysis.
    
# Contact Information
For any questions or issues regarding the project, feel free to contact:

# Mohammad Shueb

Email: mohammedshueb20525@gmail.com
