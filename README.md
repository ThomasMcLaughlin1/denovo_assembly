#  Description - Genome Assembly Pipeline 

A series of shell scripts designed for genome assembly from de novo sequencing data. This pipeline integrates multiple tools to merge, assess, assemble, and visualize genomic data from Nanopore and Illumina platforms.

# Contents

- [About](#about)
- [Features](#features)
- [Prerequisites](#Prerequisites)
- [Installation](#installation)
- [Installing prerequisites](#Installing_prerequisites)
- [Usage](#usage)
- [Customization](#customization)
- [Contributing](#contributing)
- [License](#license)

#About

This github page is desgined to showcase the scripts used to assemble and analyse nanopore and illumina reads from the species Haloferax volcanii. This pipeline enabled the sucessful identification of genomic changes within the samples provided, as well as providing detailed insights into chromosomal structure. 



#Features

- Merges Nanopore (long reads) and Illumina (short reads) data

- Quality assessment with NanoPlot

- Assembly using Unicycler

- Visualisation of prokaryotic long read, short read and hybrid assemblies usi Genovi

- comparative analysis of assemblies using QUAST

- Annotation of assemblies using PROKKA

- Visualisation of annotation using Artemis

- Mapping of short reads to reference using BWA

- Mapping of long reads to reference using minimap2

- Visualization of reads mapped back to reference in IGV

# Prerequisites

Ensure the following dependencies are installed:

NanoPlot

Unicycler

QUAST

Minimap2

BWA

Artemis


# Installation

git clone https://github.com/ThomasMcLaughlin1/denovo_assembly.git
cd genome-assembly-pipeline

# Installing prerequisites 
conda install -c bioconda nanoplot unicycler quast minimap2 bwa

# Usage 
All SLURM scripts were submitted to the University of Nottingham's HPC. Running and moitoring jobs were done by using the following commands 
- Submitting a job: sbatch <script_name>
- moniter jobs progress: squeue -l -u <username>
- cancel job: scancel <jobID>

# Contributing
Contributions are welcome! Please open an issue or submit a pull request.


