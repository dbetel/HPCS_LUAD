# HPCS_LUAD
Code base for high-plasticity cell state in lung adenocarcinoma study by Chan*, Pan* et. al. 

_Requirements_: SCANPY, AnnData, Scipy

## Part 1 - Processing of 10x Single Cell Mouse Sequencing Data (recommended to run these in the order shown).

All generated sequencing data and count matrices are available at the NCBI Gene-Expression Omnibus under accession record GSE277777.

_Part1.conda.env_ - Conda package list used to analyze data from Part 1. Use "conda create --name <env> --file Part1.conda.env" to recreate the environment used to analyze the data in from this section.  Data originally run on a conda environment within an Intel Mac OS X environment.

**_Marjanovic\_et\_al\_2020_** - Contains the Jupyter notebook to process the data from Marjanovic*, Hofree*, Chan* et al., Cancer Cell 2020. A prerequisite to classify the cell states required to generate the figures in the paper.

**_IGO14143_-Validation of Reporter** - Contains the Jupyter notebook to process FACS sorted 16 week KP Slc4a11-MCD/+ Hipp11-GGCB/+ tumors traced for 2 weeks post Tamoxifen. Generates data for Figure 1h, validation of the Slc4a11-MCD reporter.  

**_tracing_** - Contains the Jupyter notebooks to process KP Slc4a11-MCD/+ Rosa26-mTmG/+ tumors used in tracing experiments.  
   1. **_IGO15600_** - Contains the Jupyter notebook to process FACS sorted 14 week KP Slc4a11-MCD/+ Rosa26-mTmG/+ tumors traced for 2 weeks post Tamoxifen.  
   2. **_IGO15601_** - Contains the Jupyter notebook to process FACS sorted 8 week KP Slc4a11-MCD/+ Rosa26-mTmG/+ tumors traced for 2 weeks post Tamoxifen.  
   3. **_IGO15771_** - Contains the Jupyter notebook to process FACS sorted 14 week KP Slc4a11-MCD/+ Rosa26-mTmG/+ tumors traced for 2 weeks post Tamoxifen.  
   4. **_IGO15600\_IGO15601\_IGO15771\_combined_** - Contains the Jupyter notebook to concatenate IGO15600, IGO15601, and IGO15771. Run after processing the code in IGO15600, IGO15601, and IGO15771.

**_untraced_control_** - Contains Jupyter notebooks to process KPT tumors that are untraced.  
  1. **_IGO15488\_1_** - Contains the Jupyter notebook to process FACS sorted 14 week KP Rosa26-tdTomato/+ tumors.  
  2. **_IGO15488\_2_** - Contains the Jupyter notebook to process FACS sorted 14 week KP Rosa26-tdTomato/+ tumors.  
  3. **_IGO15488\_1\_2\_combined_** - Contains the Jupyter notebook to concatenate IGO15488\_1 and IGO15488\_2. Run after processing the code in IGO15488\_1 and IGO15488\_2.  
 
**_depletion_** - Contains the Jupyter notebooks to process KP Slc4a11-MCD/+ Rosa26-GGCB/+ tumors ablated using diphtheria toxin.  
   1. **_IGO15123_** - Contains the Jupyter notebook to process FACS sorted 16 week KP Slc4a11-MCD/+ Rosa26-GGCB/+ tumors ablated for 1 weeks via diphitheria toxin treatment.  
   2. **_IGO15342_** - Contains the Jupyter notebook to process FACS sorted 16 week KP Slc4a11-MCD/+ Rosa26-GGCB/+ tumors ablated for 1 weeks via diphtheria toxin treatment.  
   3. **_IGO15123\_IGO15342\_combined_** - Contains the Jupyter notebook to concatenate IGO15123 and IGO15342. Run after processing the code in IGO15123 and IGO15342.

**_IGO16235-Drug treatment experiments_** - Contains the Jupyter notebook to process FACS sorted 17 week KP Slc4a11-MCD/+ Rosa26-mTmG/+ tumors lineage traced with Tamoxifen and treated with either vehicle, cisplatin, or MRTX1133 for 3 weeks. Generates data for Figure 4c,d. Note: code to generate data for Figure 4c is commented out by default given long runtime.  

**_IGO16318-Hopx-MACD-validation_** - Contains the Jupyter notebook to process FACS sorted 16 week KPfrt Hopx-MACD/+ Hipp11-GGCB/+ tumors. Generates data for Extended Data Figures 6h-j.  

**_Slc4a11\_tracing\_depletion\_analysis_** - Contains the Jupyter notebooks to process depletion cohort (IGO15123\_IGO15342\_combined), traced cohort (IGO15600\_IGO15601\_IGO15771), and untraced control (IGO15488_1_2) in a uniform manner. Generates data for Fig 1, 2, and 4, as well as Extended Data Fig 4, 5, and 7.

## Part 2 - Processing of previously published scRNA-seq data
