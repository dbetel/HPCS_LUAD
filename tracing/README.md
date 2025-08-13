# HPCS_LUAD
Code base for high-plasticity cell state in lung adenocarcinoma study by Chan*, Pan* et. al. 

_Requirements_: SCANPY, AnnData, Scipy

## Part 1 - Processing of 10x Single Cell Mouse Sequencing Data (recommended to run these in the order shown).

All generated sequencing data and count matrices are available at the NCBI Gene-Expression Omnibus under accession record GSE277777.

Process and combine the lanes used in the 3d and 14d tracing experiments from _KPfrt Slc4a11<sup>MCD/+</sup> or KPfrt Hopx<sup>MACD/+</sup> Rosa26<sup>mTmG/+</sup>_ tumors.

**_IGO15600_** - Contains the Jupyter notebook to process FACS sorted 14 week _KP Slc4a11<sup>MCD/+</sup> Rosa26<sup>mTmG/+</sup>_ tumors traced for 2 weeks post Tamoxifen.  

**_IGO15601_** - Contains the Jupyter notebook to process FACS sorted 8 week _KP Slc4a11<sup>MCD/+</sup> Rosa26<sup>mTmG/+</sup>_ tumors traced for 2 weeks post Tamoxifen.  

**_IGO15771_** - Contains the Jupyter notebook to process FACS sorted 14 week _KP Slc4a11<sup>MCD/+</sup> Rosa26<sup>mTmG/+</sup>_ tumors traced for 2 weeks post Tamoxifen.   

**_IGO16686_** - Contains the Jupyter notebook to process FACS sorted 12 week + 3 days _KP Slc4a11<sup>MCD/+</sup> Rosa26<sup>mTmG/+</sup>_ tumors traced for 3 days post Tamoxifen.   

**_IGO17402_** - Contains the Jupyter notebook to process FACS sorted 6 week + 3 days _KP Slc4a11<sup>MCD/+</sup> Rosa26<sup>mTmG/+</sup>_ tumors traced for 3 days post Tamoxifen.  Also contains FACS sorted 12 week + 3 days _KP Hopx<sup>MACD/+</sup> Rosa26<sup>mTmG/+</sup>_ tumors traced for 3 days post Tamoxifen. 

**_IGO17543.ipynb_** - Contains the Jupyter notebook to process KPfrt Hopx-MACD/+ Rosa26-mTmG/+ tumors harvested 12 weeks post tumor induction after 14 days of tracing induction with Tamoxifen.

**_IGO15600\_IGO15601\_IGO15771\_IGO16686\_IGO17402\_IGO17543\_combined_** - Contains the Jupyter notebook to concatenate IGO15600, IGO15601, IGO15771, IGO16686, IGO17402, and IGO17543. Run after processing the code in IGO15600, IGO15601, IGO15771, IGO16686, IGO17402, and IGO17543.  
