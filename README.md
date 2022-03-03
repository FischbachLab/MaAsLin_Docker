# MaAsLin_Docker

This is a MaAsLin2 docker image with Bioconductor and RStudio based on [bioconductor_docker] (https://github.com/Bioconductor/bioconductor_docker) 

MaAsLin2 (https://github.com/biobakery/Maaslin2) is comprehensive R package for efficiently determining multivariable association with Linear Models.


## Run a MaAsLin demo dataset within a docker container
```bash
/work/Maaslin2-1.7.3/R/Maaslin2.R \
    --transform=AST \
    --fixed_effects="diagnosis,dysbiosisnonIBD,dysbiosisUC,dysbiosisCD,antibiotics,age" \
    --random_effects="site,subject" \
    --normalization=NONE \
    --standardize=FALSE \
    --reference="diagnosis,nonIBD" \
    /work/Maaslin2-1.7.3/inst/extdata/HMP2_taxonomy.tsv \
    /work/Maaslin2-1.7.3/inst/extdata/HMP2_metadata.tsv \
    demo_output
```
