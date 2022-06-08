# RNApipe
 Easy and quick pipeline for RNAseq analysis

## Quick Start
1. -STEP01:
	-INSTALL NEXTFLOW FOR PIPELINE: 
	```bash
	curl -s https://get.nextflow.io | bash  OR INSTALL WITH CONDA : conda install nextflow 
	```
	-This pipeline is based on nextflow DSL2 , so you can run nextflow self-update to update NEXTFLOW to new version

2. -STEP02:
	-CONDA ENVIRONMENT DEPLOY:
	```bash
	conda env create -f environment.yaml
	```
	-This code will create a conda environment for wgs/wes analysis named onestep_rnaseq
3. -STEP03:
	-RUN PIPELINE:
	```bash
	nextflow run main.nf --genome genome.fa --gtf genes.gtf --hisat2_index /index/genome --reads 'reads/*_{1,2}.fq.gz' --with-conda /path/to/onestep_rnaseq
	```
