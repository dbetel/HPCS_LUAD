# HPCS_LUAD
Code base for high-plasticity cell state in lung adenocarcinoma study by Chan*, Pan* et. al. 

_Requirements_: SCANPY, AnnData, Scipy

## Processing of 10x Single Cell Mouse Sequencing Data (recommended to run these in the order shown).

_Marjanovic\_et\_al\_2020_ - Contains the Jupyter notebook to process the data from Marjanovic*, Hofree*, Chan* et al., Cancer Cell 2020. A prerequisite to classify the cell states required to generate the figures in the paper.  
_IGO14143_ - Contains the Jupyter notebook to process FACS sorted 16 week KPfrt Slc4a11-MCD/+ Hipp11-GGCB/+ tumors traced for 2 weeks post Tamoxifen. Generates data for Figure 1h.  
_IGO15600_ - Contains the Jupyter notebook to process FACS sorted 14 week KPfrt Slc4a11-MCD/+ Rosa26-mTmG/+ tumors traced for 2 weeks post Tamoxifen.  
_IGO15601_ - Contains the Jupyter notebook to process FACS sorted 8 week KPfrt Slc4a11-MCD/+ Rosa26-mTmG/+ tumors traced for 2 weeks post Tamoxifen.  
_IGO15771_ - Contains the Jupyter notebook to process FACS sorted 14 week KPfrt Slc4a11-MCD/+ Rosa26-mTmG/+ tumors traced for 2 weeks post Tamoxifen.  
_IGO15600\_IGO15601\_IGO15771\_combined_ - Contains the Jupyter notebook to concatenate IGO15600, IGO15601, and IGO15771. Run after processing the code in IGO15600, IGO15601, and IGO15771.  
_IGO15123_ - Contains the Jupyter notebook to process FACS sorted 16 week KPfrt Slc4a11-MCD/+ Rosa26-GGCB/+ tumors ablated for 1 weeks via Diptheria toxin treatment.  
_IGO15342_ - Contains the Jupyter notebook to process FACS sorted 16 week KPfrt Slc4a11-MCD/+ Rosa26-GGCB/+ tumors ablated for 1 weeks via Diptheria toxin treatment.  
_IGO15123\_IGO15342\_combined_ - Contains the Jupyter notebook to concatenate IGO15123 and IGO15342. Run after processing the code in IGO15123 and IGO15342.  
_IGO16235_ - Contains the Jupyter notebook to process FACS sorted 17 week KPfrt Slc4a11-MCD/+ Rosa26-mTmG/+ tumors lineage traced with Tamoxifen and treated with either vehicle, cisplatin, or MRTX1133 for 3 weeks. Generates data for Figure 4c,d. Note: code to generate data for Figure 4c is commented out by default given long runtime.  
_IGO16318_ - Contains the Jupyter notebook to process FACS sorted 16 week KPfrt Hopx-MACD/+ Hipp11-GGCB/+ tumors. Generates data for Extended Data Figures 6h-j.  
_IGO15488\_1_ - Contains the Jupyter notebook to process FACS sorted 14 week KP Rosa26-tdTomato/+ tumors.  
_IGO15488\_2_ - Contains the Jupyter notebook to process FACS sorted 14 week KP Rosa26-tdTomato/+ tumors.  
_IGO15488\_1\_2\_combined_ - Contains the Jupyter notebook to concatenate IGO15488\_1 and IGO15488\_2. Run after processing the code in IGO15488\_1 and IGO15488\_2.  
_Slc4a11\_tracing\_depletion\_analysis_ - Contains the Jupyter notebook to process depletion cohort (IGO15123\_IGO15342\_combined), traced cohort (IGO15600\_IGO15601\_IGO15771), and untraced control (IGO15488_1_2) in a uniform manner. Generates data for Fig 1, 2, and 4, as well as Extended Data Fig 4, 5, and 7.
