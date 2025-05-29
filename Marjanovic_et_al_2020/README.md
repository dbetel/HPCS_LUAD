# HPCS_LUAD - Marjanovic*, Hofree*, Chan*, et al. Cancer Cell 2020
Part of the code base for analysis of the high-plasticity cell state in lung adenocarcinoma study by Chan*, Pan* et. al. 

## Processing of SmartSeq2 data from Marjanovic*, Hofree*, and Chan* et. al., Cancer Cell 2020 to generate a logistic regression model for cell state classification. 

Note: Run Jupyter-notebooks in the following order (requires data from GSE154989 to be placed in a directory 'data' found in the main folder).

**_01_makeLuadAdata.ipynb_** - Jupyter notebook to process data from Marjanovic*, Hofree*, and Chan* et. al., Cancer Cell 2020 (GSE154989). 

**_02_Marjanovic.ipynb_** - Jupyter notebook creates the ../common_files/genes.joblib used to help classify tumor cells in IGO14143, IGO15600, IGO15601, IGO15123, IGO15342, IGO16235, and IGO16318.
