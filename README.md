# Variant Calling Pipeline

This project was developed as a learning exercise to understand the variant calling process using high-throughput sequencing data. It covers each step from raw data quality control to variant visualization using standard bioinformatics tools.

## Workflow Overview

1. **Quality Control**
   - *FastQC* is used to assess the quality of raw sequencing reads.

2. **Read Alignment**
   - *Minimap2* aligns reads to the reference genome, generating a SAM file.

3. **File Conversion and Processing**
   - *SAMtools* converts the SAM file to BAM, then sorts and indexes it.

4. **Duplicate Marking**
   - *Picard* or *SAMtools* marks duplicate reads to prevent bias in downstream analysis.

5. **Base Quality Score Recalibration (BQSR)**
   - *GATK* recalibrates base quality scores to improve the accuracy of variant calls.

6. **Variant Calling**
   - *GATK HaplotypeCaller* identifies SNPs and Indels and outputs them in VCF format.

7. **Visualization**
   - *IGV* is used to visually inspect alignment and variant data.

## Tools Used

- FastQC  
- Minimap2  
- SAMtools  
- Picard  
- GATK  
- IGV  

