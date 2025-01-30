# AmpWrap
A powerful workflow for the analysis of short and long 16S rRNA amplicons.

## Table of Contents
- [Introduction](#introduction)
- [Installation with Conda](#installation-with-conda)
  - [Install Miniconda](#install-miniconda)
  - [Install Mamba](#install-mamba)
  - [Install AmpWrap](#install-ampwrap)
- [Usage](#usage)
  - [AmpWrap for Short Reads (Illumina)](#ampwrap-for-short-reads-illumina)
  - [AmpWrap for Long Reads (Nanopore)](#ampwrap-for-long-reads-nanopore)
- [Troubleshooting](#troubleshooting)

## Introduction
AmpWrap is a streamlined and efficient workflow for the analysis of 16S rRNA amplicons, supporting both short-read (Illumina) and long-read (Nanopore) sequencing technologies.

## Installation with Conda
AmpWrap can be easily installed using Conda or Mamba.

### Install Miniconda
To use Conda or Mamba, you first need to install Miniconda:

```sh
mkdir -p ~/miniconda3
wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh -O ~/miniconda3/miniconda.sh
```

Run the installation script:
```sh
bash ~/miniconda3/miniconda.sh -b -u -p ~/miniconda3
source ~/.bash_profile || source ~/.bashrc
```

After installation, remove the installer to free up space:
```sh
rm -rf ~/miniconda3/miniconda.sh
```

### Install Mamba
Mamba is a faster alternative to Conda for package management. Install it with:

```sh
conda install -n base -c conda-forge mamba
```

### Install AmpWrap
You can install AmpWrap using either Conda or Mamba:

```sh
conda install -c bioconda ampwrap
```

or using Mamba:

```sh
mamba install -c bioconda ampwrap
```

## Usage

### AmpWrap for Short Reads (Illumina)
To process short-read 16S rRNA data from Illumina sequencing, use:

```sh
ampwrap illumina -i input_directory -o output_directory
```

### AmpWrap for Long Reads (Nanopore)
For long-read 16S rRNA data from Nanopore sequencing, use:

```sh
ampwrap nanopore -i input_directory -o output_directory
```

## Troubleshooting
If you encounter issues during installation or execution, check the following:
- Ensure that Conda/Mamba is properly installed and activated.
- Verify that AmpWrap is installed in the correct Conda environment.
- Check the logs for error messages and missing dependencies.

For further assistance, refer to the official documentation or community forums.



 

