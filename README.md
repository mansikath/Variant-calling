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

---

Copyright (c) 2024 Mansi Kathrotiya

All rights reserved.

Permission is hereby NOT granted to any person or organization to use, copy, modify, merge, publish, distribute, sublicense, or sell copies of the software or associated files without prior written consent from the author.

Unauthorized use, reproduction, or distribution of any part of this repository is strictly prohibited and may result in legal action.

If you wish to use any part of this project for educational, research, or commercial purposes, please contact:

Mansi Kathrotiya  
Email: mkathrotiya812@email.com  
GitHub: https://github.com/mansikath  
LinkedIn: https://linkedin.com/in/mansi  

This license applies to all files and content within this repository.