# HPCS_LUAD
Code base for high-plasticity cell state in lung adenocarcinoma study by Chan*, Pan* et. al. 

_Requirements_: SCANPY, AnnData, Scipy

## Part 1 - Processing of 10x Single Cell Mouse Sequencing Data (recommended to run these in the order shown).

All generated sequencing data and count matrices are available at the NCBI Gene-Expression Omnibus under accession record GSE277777.

The code in these subdirectories are meant to preprocess the scRNA-seq sequencing data from depletion experiments which used diphtheria toxin.

**_IGO15123_** - Contains the Jupyter notebook to process FACS sorted 16 week _KP Slc4a11<sup>MCD/+</sup> Rosa26<sup>GGCB/+</sup>_ tumors ablated for 1 weeks via diphtheria toxin treatment.  

**_IGO15342_** - Contains the Jupyter notebook to process FACS sorted 15 week _KP Slc4a11<sup>MCD/+</sup> Rosa26<sup>GGCB/+</sup>_ tumors ablated for 1 week via diphtheria toxin treatment.  

**_IGO15123\_IGO15342\_combined_** - Contains the Jupyter notebook to concatenate IGO15123 and IGO15342. Run after processing the code in IGO15123 and IGO15342.  
