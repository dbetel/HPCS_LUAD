# HPCS_LUAD
Code base for high-plasticity cell state in lung adenocarcinoma study by Chan*, Pan* et. al. 

_Requirements_: SCANPY, AnnData, Scipy

## Part 1 - Processing of 10x Single Cell Mouse Sequencing Data (recommended to run these in the order shown).

All generated sequencing data and count matrices are available at the NCBI Gene-Expression Omnibus under accession record GSE277777.

Process and combine the lanes used in the IV transplant model of a _KPfrt Slc4a11<sup>MACD/+</sup>_ cell line.

**_IGO17483_** - Contains the Jupyter notebook to process FACS sorted IV transplanted _KPfrt Slc4a11<sup>MACD/+</sup>_ cells treated with Saline or DT for 7 days. Run the IGO17483-Vehicle and IGO17483-DT notebooks before running the combined notebook.  Generates data for Extended Data Fig. 9n.