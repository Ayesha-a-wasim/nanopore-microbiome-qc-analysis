# 🧬 Nanopore Microbiome Analysis Pipeline
This project contains a complete pipeline for processing Nanopore sequencing data, focused on microbiome analysis.

🎯 Developed as part of my PhD research on microbiota and colorectal cancer.

---

## 🔍 What This Pipeline Does
- Sets up conda environment and installs all required tools
- Performs quality control using NanoFilt, NanoStat, and NanoPlot
- Prepares data for QIIME2 (renaming, compression, and manifest file creation)
- Imports data into QIIME2 for analysis
- Denoises sequences using DADA2
- Assigns taxonomy using pretrained classifiers
- Builds phylogenetic trees
- Computes diversity metrics (alpha/beta)
- Visualizes results (bar plots, diversity stats)
- Exports data for downstream analysis

---

## 🧰 Tools Used
- QIIME2
- NanoFilt / NanoStat / NanoPlot
- Porechop / Cutadapt
- Minimap2
- SAMtools / BCFtools / HTSlib
- Medaka / Nanopolish / pycoQC
- Picard / GATK
- SRA Toolkit
- R + R Markdown

---

## 📁 Project Structure
nanopore_pipeline/ ├── reads/ # FASTQ input files ├── taxonomy/ # Taxonomy reference files ├── metadata/ # Metadata CSV/TSV files ├── features/ # Feature tables (e.g. BIOM) ├── output/ # All QIIME2 analysis results ├── nbin/ # Custom bin directory for tools └── nanopore_pipeline.Rmd # Main analysis document


---

## 🚀 How to Use

1. Clone the repository:
```bash
git clone https://github.com/yourusername/nanopore-microbiome-analysis.git
cd nanopore-microbiome-analysis

2. Open the R Markdown file in RStudio or any R environment.

3. Follow the steps in the .Rmd file
Set up your environment
Install tools
Run QC on FASTQ files
Import into QIIME2
Perform taxonomy and diversity analysis

4. Use generated .qzv files to explore interactive results.

📌 Notes
This pipeline is built for single-end Nanopore reads.
Compatible with QIIME2 SingleEndFastqManifestPhred33V2 format.
Ensure your system has the required permissions and paths correctly set up.

🧑‍🔬 Author
Ayesha Wasim
PhD Fellow – Marie Skłodowska-Curie Actions
Universidade da Coruña, Spain
📫 ayesha.wasim@udc.es


