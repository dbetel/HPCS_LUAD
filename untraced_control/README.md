# HPCS_LUAD
Code base for high-plasticity cell state in lung adenocarcinoma study by Chan*, Pan* et. al. 

_Requirements_: SCANPY, AnnData, Scipy

## Part 1 - Processing of 10x Single Cell Mouse Sequencing Data (recommended to run these in the order shown).

All generated sequencing data and count matrices are available at the NCBI Gene-Expression Omnibus under accession record GSE277777.

This directory preprocesses the scRNA-seq sequencing data from KPT tumors that are untraced. Jupyter-notebooks are meant to run in the order listed below.

**_IGO15488\_1_** - Contains the Jupyter notebook to process FACS sorted 14 week _KP Rosa26<sup>tdTomato/+</sup>_ tumors.

**_IGO15488\_2_** - Contains the Jupyter notebook to process FACS sorted 14 week _KP Rosa26<sup>tdTomato/+</sup>_ tumors.  

**_IGO15488\_1\_2\_combined_** - Contains the Jupyter notebook to concatenate IGO15488\_1 and IGO15488\_2. Run after processing the code in IGO15488\_1 and IGO15488\_2.  

