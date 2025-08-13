# HPCS_LUAD
Part of the code base for analysis of the high-plasticity cell state in lung adenocarcinoma study by Chan*, Pan* et. al. 

## Processing of 10x single cell mRNA sequencing data generated from tumors below.  Cells were hashed using mouse TotalSeq B hashes as per Stoeckius et al., Genome Biology, 2018.

**_01\_Concatenate\_cells.ipynb_** - Jupyter notebook to concatenate depletion cohort (IGO15123\_IGO15342\_combined), traced cohort (IGO15600\_IGO15601\_IGO15771\_IGO16686\_IGO17402\_IGO17543), and untraced control cohort (IGO15488_1_2 and IGO16318). All items to be projected onto the same uMAP.  

**_02\_Analyze\_control\_DT\_depletion.ipynb_** - Jupyter notebook to evaluate tumor control and 7 day DT treated tumor cells. Uses depletion cohort (IGO15123\_IGO15342\_combined). Generates data for Fig 1a, 1b (similar to Extended Data Fig 4b), 1h, Extended Data Fig 4b, 9a, 10c.  

**_03\_Evaluate\_traced\_cells_Slc4a11.ipynb_** - Jupyter notebook to evaluate traced cells. Uses traced cohorts (IGO15600, IGO15601, IGO15771, IGO16686, IGO17402) and untraced control (IGO15488_1_2). Generates data for Fig 2d,f-h, Extended Data Fig 7a-e,f

**_04\_Evaluate\_traced\_cells_Hopx.ipynb_** - Jupyter notebook to evaluate traced cells. Uses traced cohorts (IGO17402, IGO17543) and untraced control (IGO16318). Generates data for Fig 2d-i, Extended Data Fig 5a-h

**_05\_Evaluate\_phenotypic\_volumes.ipynb_** - Jupyter notebook to evaluate phenotypic volume of the cohorts. Uses traced cohorts (IGO15600, IGO15601, IGO15771, IGO16686, IGO17402, IGO17543) and untraced controls (IGO15488_1_2, IGO16318). Generates data for Fig, Extended Data Fig 5a-h
