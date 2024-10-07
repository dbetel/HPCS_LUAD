# HPCS_LUAD
Code base for high-plasticity cell state in lung adenocarcinoma study by Chan*, Pan* et. al. 

_Requirements_: SCANPY, AnnData, Scipy

## Part 1 - Processing of 10x Single Cell Mouse Sequencing Data (recommended to run these in the order shown).

All generated sequencing data and count matrices are available at the NCBI Gene-Expression Omnibus under accession record GSE277777.

_Part1.conda.env_ - Conda package list used to analyze data from Part 1. Use "conda create --name <env> --file Part1.conda.env" to recreate the environment used to analyze the data in from this section.  Data originally run on a conda environment within an Intel Mac OS X environment.

![Part I](https://github.com/user-attachments/assets/c8921d66-b8d8-49bf-b5af-bd729c69074b)

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

We downloaded publicly available scRNA-seq data from mouse and human studies across different tissues including colon, skin, prostate, pancreas, and breast. Below is the breakdown of which files were used to analize the data and the corresponding figures in the publication.

Each dataset was downloaded individually then quality control and analysis was done per dataset as run in the assosiated python notebook. 

Then the information was aggregated an copmared in the hpcsQuant file to generate the figures.

### Information Table

| Tissue        | ipynb File                | Gene Signature| Figure       | PMID     |
|---------------|---------------------------|---------------|--------------|----------|
| **Mouse**     |                           |               |              |          |
| Colon         | mouseColon                | coreHRC       | 5e (2)       | 36352230 |
| Skin          | mouseSkin                 | lower spike   | 5e (4)       | 38815020 |
| Prostate      | mouseProstate             | ADENO         | 5b,c,d,e (3) | 35981096 |
| Pancreas      | mousePancreas             | Basal         | 5e (3)       | 35952360 |
| Breast        | mouseBreast               |               |              | 32840210 |
| Lung          | makeLuadAdata             | HPCS          |              | 32707077 |
| Lung          | mouseLung                 | DATP          | 5g,h         | 32750316 |
| Lung          |                           | ADI           | 5i           | 32678092 |
| Lung          |                           | PATS          | 5i           | 32661339 |
|               |                           |               |              |          |
| **Human**     |                           |               |              |          |
| Colon         | humanColorectalPelka2021  |               |              | 34450029 |
| Skin          | humanSkinJi2020           |               |              | 32579974 |
| Prostate      | humanProstateDong2020     |               |              | 33328604 |
| Pancreas      | humanPancreasSteele2020   |               |              | 34296197 |
| Breast        | humanBreastPal2021        |               |              | 33950524 |
| Lung          | humanLungMDA              | KAC           | 5f           | 38418883 |
| Lung          | humanLungKim              |               |              | 32385277 |
| Lung          | humanLungBischoff         |               |              | 34663877 |
| Lung          | humanLungDost             |               |              | 32891189 |
|               |                           |               |              |          |
| **Pan Caner** |                           |               |              |          |
| Yanai         |                           | Stress        | Ex 9         | 35931863 |
| Tirosh        |                           | Stress        | 5a           | 37258682 |





