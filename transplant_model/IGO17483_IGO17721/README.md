# HPCS_LUAD
Code base for high-plasticity cell state in lung adenocarcinoma study by Chan*, Pan* et. al. 

_Requirements_: SCANPY, AnnData, Scipy

## Part 1 - Processing of 10x Single Cell Mouse Sequencing Data (recommended to run these in the order shown).

All generated sequencing data and count matrices are available at the NCBI Gene-Expression Omnibus under accession record GSE277777.

Process and combine the lanes used in the IV transplant model of a _KPfrt Slc4a11<sup>MCD/+</sup>_ and _KPfrt Hopx<sup>MACD/+</sup>_ cell lines.

**_IGO17483\_IGO17721.ipynb_** Calculates phenotypic volume and generates data for Extended Data Fig. 9n.
