# HPCS_LUAD
Code base for high-plasticity cell state in lung adenocarcinoma study by Chan*, Pan* et. al. 

_Requirements_: SCANPY, AnnData, Scipy

## Part 1 - Processing of 10x Single Cell Mouse Sequencing Data (recommended to run these in the order shown).

All generated sequencing data and count matrices are available at the NCBI Gene-Expression Omnibus under accession record GSE277777.

The code in these subdirectories are meant to preprocess the scRNA-seq sequencing data from depletion experiments which used diphtheria toxin.

**_IGO16235.ipynb_** - Jupyter notebook to process _KP Slc4a11<sup>MCD/+</sup> Rosa26<sup>mTmG/+</sup>_ tumors harvested 17 weeks post tumor induction after 3 weeks of lineage tracing post Tamoxifen under therapeutic pressure with either vehicle, cisplatin, or MRTX1133.

**_IGO16562.ipynb_** - Jupyter notebook to process _KP Slc4a11<sup>MCD/+</sup> Rosa26<sup>mTmG/+</sup>_ tumors harvested 17 weeks post tumor induction after 3 weeks of lineage tracing post Tamoxifen under therapeutic pressure with either vehicle, cisplatin, or MRTX1133.

**_IGO16235\_IGO16562\_combined_** - Contains the Jupyter notebook to concatenate IGO16235 and IGO16562. Run after processing the code in IGO16235 and IGO16562.  
