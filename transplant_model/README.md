# HPCS_LUAD
Code base for high-plasticity cell state in lung adenocarcinoma study by Chan*, Pan* et. al. 

_Requirements_: SCANPY, AnnData, Scipy

## Part 1 - Processing of 10x Single Cell Mouse Sequencing Data (recommended to run these in the order shown).

All generated sequencing data and count matrices are available at the NCBI Gene-Expression Omnibus under accession record GSE277777.

Process and combine the lanes used in the IV transplant model.

**_IGO17483_** - Contains the Jupyter notebook to process FACS sorted IV transplanted _KPfrt Slc4a11<sup>MCD/+</sup>_ cells treated with Saline or DT for 7 days.

**_IGO17721_** - Contains the Jupyter notebook to process FACS sorted IV transplanted _KPfrt Hopx<sup>MACD/+</sup>_ cells treated with Saline or DT for 7 days.

**_IGO17483\_IGO17721_** - Contains the Jupyter notebook to concatenate and process FACS sorted IV transplanted _KPfrt Slc4a11<sup>MCD/+</sup>_ cells (IGO17483) and _KPfrt Hopx<sup>MACD/+</sup>_ cells (IGO17721). Run after processing IGO17483 and IGO17721.
