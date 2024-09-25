# HPCS_LUAD
Part of the code base for analysis of the high-plasticity cell state in lung adenocarcinoma study by Chan*, Pan* et. al. 

## Processing of 10x single cell mRNA sequencing data generated from tumors below.  Cells were hashed using mouse TotalSeq B hashes as per Stoeckius et al., Genome Biology, 2018.

_01\_Concatenate\_cells.ipynb_ - Jupyter notebook to concatenate depletion cohort (IGO15123\_IGO15342\_combined), traced cohort (IGO15600\_IGO15601\_IGO15771), and untraced control (IGO15488_1_2). All items to be projected onto the same uMAP.
_02\_Analyze\_control\_DT\_depletion.ipynb_ - Jupyter notebook to evaluate tumor control and 7 day DT treated tumor cells. Uses depletion cohort (IGO15123\_IGO15342\_combined). Generates data for Fig 1i,4g, Extended Data Fig 4b,5g,7c.
_03\_Evaluate\_traced\_cells.ipynb_ - Jupyter notebook to evaluate traced cells. Uses traced cohort (IGO15600\_IGO15601\_IGO15771) and untraced control (IGO15488_1_2). Generates data for Fig 2d-i, Extended Data Fig 5a-h
