# SMK_ATAC

This workflow performs data process for ATAC-seq from fastq to call peaks by MACS2


## Workflow



![dag1](https://github.com/mhu10/SMK_ATAC/assets/38729968/f37c79df-c695-4bdd-8c31-d31765771dbb)




## Install Snakemake and Git

Please make sure that Snakemake and Git are correctly installed

Snakemake: https://snakemake.readthedocs.io/en/stable/getting_started/installation.html

Git: https://anaconda.org/anaconda/git



## clone workflow into working directory

```
git clone https://github.com/mhu10/SMK_ATAC path/to/workdir
```


## Edit config file and workfileas as needed

./SMK_ATACseq/config/'config.yaml

./SMK_ATACseq/Snakefile

## Activate snakemake

```
conda activate snakemake
```

## Dry run workflow

```
snakemake -n
```

## Execute workflow

```
snakemake --use-conda --cores 12
```

## Build DAG workflow chart

```
snakemake --rulegraph | dot -Tsvg > dag1.svg
```
