# The genomic footprint of sexual conflict -- supplementary data and scripts
This is a collaborative project between the [Göran Arnqvist group](http://arnqvist.org/), Animal Ecology, Dept. of Ecology and Genetics, Uppsala University and the [NBIS](https://nbis.se/) long-term support (a.k.a. WABI), performed during 2015-2018 (NBIS LT project name: G_Arnqvist_1305).

As a part of the NBIS reproducible research policy, this repository provides the data-files and R-scripts necessary to perform the underlying analyses and create tables and plots used in Sayadi et al. The genomic footprint of sexual conflict (manuscript in prep; link not yet available)

Several scripts where provided to reproduces most parts of the Pool-Seq analysis. Please refer to the readme file for more details.

*Note! The repository is provided for reproducibility reasons, only; no further development will be made.*

## Usage
#### Download
The content of this repository can be obtained in two ways:
*	Download the current release as a zip- or tar-archive (e.g., by clicking `Download Zip File` or `Download TAR Ball` on `thegithub.io page`)
*	Clone the repository from the github page (reached from the `github.io` page by clicking `View on GitHub`)

#### Running the scripts

## Repository content:
* **README.md** This file.

## Folders
** Genome Assembly**
** Genome Annotation**
**Popoolation**
In this directory you will find two shell scripts that should be used to reproduce the SNP file (Popoolation output file tool).
1- first you need to run PopoolationPart1.sh and then PopoolationPart2.sh
several modules need to be installed (Python, bowtie2, smatools, bcftools, bwa, java, picard).
Raw file data need to be downloaded: (Genome assembly file, raw sequencing data).
The annotated genome assembly, along with sequence data, is available from the European Nucleotide Archive (ENA) under accession PRJEB30475.
All Pool-seq raw sequencing data have been deposited at the NCBI sequence read archive, under the accession number PRJNA503561.
Please modify the script according to your folder organisation.
several folders need to be created before runing the script (place your sheel script in the same directory):
```
# Creating necessary folders
mkdir ref # place genome asembly file in this folder
mkdir reads # place raw reads in this folder
mkdir trimmed.reads
mkdir mapping
# please modify the first 2 lines in the bash script PoPoolationPart1.sh to include the reference genome and the raw reads.
bash PoPoolationPart1.sh
bash PoPoolationPart2.sh
```
### 

## Contact
* Göran Arnqvist group, UU:
     - [Ahmed Sayadi](mailto:ahmed.sayadi@ebc.uu.se)
     - [Göran Arnqvist](mailto:Goran.Arnqvist@ebc.uu.se)
* NBIS long-term support:
     - [Björn Nystedt](mailto:bjorn.nystedt@scilifelab.se)

