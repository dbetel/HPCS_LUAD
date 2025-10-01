# HPCS_LUAD
Code base for high-plasticity cell state in lung adenocarcinoma study by Chan*, Pan* et. al. 

_Requirements_: SCANPY, AnnData, Scipy

## Part 1 - Processing of 10x Single Cell Mouse Sequencing Data (recommended to run these in the order shown).

All generated sequencing data and count matrices are available at the NCBI Gene-Expression Omnibus under accession record GSE277777.

_Part1.conda.env_ - Conda package list used to analyze data from Part 1. Use "conda create --name <env> --file Part1.conda.env" to recreate the environment used to analyze the data in from this section.  Data originally run on a conda environment within an Intel Mac OS X environment.

![Part I Summary Image](Part1_Overview.png)

**_Marjanovic\_et\_al\_2020_** - Contains the Jupyter notebook to process the data from Marjanovic*, Hofree*, Chan* et al., Cancer Cell 2020. A prerequisite to classify the cell states required to generate the figures in the paper. Creates data for Extended Data Fig. 6 and 13.

**_IGO14143_-Validation of Reporter** - Contains the Jupyter notebook to process FACS sorted 16 week _KP Slc4a11<sup>MCD/+</sup> Hipp11<sup>GGCB/+<sup>_ tumors traced for 2 weeks post Tamoxifen. Generates data for Figure 1, validation of the _Slc4a11<sup>MCD/+</sup>_ reporter.  

**_tracing_** - Contains the Jupyter notebooks to process _KP Slc4a11<sup>MCD/+</sup> Rosa26<sup>mTmG/+</sup>_ tumors used in tracing experiments.  
   1. **_IGO15600_** - Contains the Jupyter notebook to process FACS sorted 14 week _KP Slc4a11<sup>MCD/+</sup> Rosa26<sup>mTmG/+</sup>_ tumors traced for 2 weeks post Tamoxifen.  
   2. **_IGO15601_** - Contains the Jupyter notebook to process FACS sorted 8 week _KP Slc4a11<sup>MCD/+</sup> Rosa26<sup>mTmG/+</sup>_ tumors traced for 2 weeks post Tamoxifen.  
   3. **_IGO15771_** - Contains the Jupyter notebook to process FACS sorted 14 week _KP Slc4a11<sup>MCD/+</sup> Rosa26<sup>mTmG/+</sup>_ tumors traced for 2 weeks post Tamoxifen.  
   4. **_IGO16686_** - Contains the Jupyter notebook to process FACS sorted 12 week + 3 days _KP Slc4a11<sup>MCD/+</sup> Rosa26<sup>mTmG/+</sup>_ tumors traced for 3 days post Tamoxifen.
   5. **_IGO17402_** - Contains the Jupyter notebook to process FACS sorted 6 week + 3 days _KP Slc4a11<sup>MCD/+</sup> Rosa26<sup>mTmG/+</sup>_ tumors traced for 3 days post Tamoxifen.  Also contains FACS sorted 12 week + 3 days _KP Hopx<sup>MACD/+</sup> Rosa26<sup>mTmG/+</sup>_ tumors traced for 3 days post Tamoxifen.
   6. **_IGO17543_** - Contains the Jupyter notebook to process KPfrt Hopx-MACD/+ Rosa26-mTmG/+ tumors harvested 12 weeks post tumor induction after 14 days of tracing induction with Tamoxifen.
   7. **_IGO15600\_IGO15601\_IGO15771\_IGO16686\_IGO17402\_IGO17543\_combined_** - Contains the Jupyter notebook to concatenate IGO15600, IGO15601, and IGO15771. Run after processing the code in IGO15600, IGO15601, and IGO15771.

**_untraced_control_** - Contains Jupyter notebooks to process _KPT_ tumors that are untraced.  
  1. **_IGO15488\_1_** - Contains the Jupyter notebook to process FACS sorted 14 week _KP Rosa26<sup>tdTomato/+</sup>_ tumors.  
  2. **_IGO15488\_2_** - Contains the Jupyter notebook to process FACS sorted 14 week _KP Rosa26<sup>tdTomato/+</sup>_ tumors.  
  3. **_IGO15488\_1\_2\_combined_** - Contains the Jupyter notebook to concatenate IGO15488\_1 and IGO15488\_2. Run after processing the code in IGO15488\_1 and IGO15488\_2.  
 
**_depletion_** - Contains the Jupyter notebooks to process _KP Slc4a11<sup>MCD/+</sup> Rosa26<sup>GGCB/+</sup>_ tumors ablated using diphtheria toxin.  
   1. **_IGO15123_** - Contains the Jupyter notebook to process FACS sorted 16 week _KP Slc4a11<sup>MCD/+</sup> Rosa26<sup>GGCB/+</sup>_ tumors ablated for 1 week via diphitheria toxin treatment.  
   2. **_IGO15342_** - Contains the Jupyter notebook to process FACS sorted 15 week _KP Slc4a11<sup>MCD/+</sup> Rosa26<sup>GGCB/+</sup>_ tumors ablated for 1 week via diphtheria toxin treatment.  
   3. **_IGO15123\_IGO15342\_combined_** - Contains the Jupyter notebook to concatenate IGO15123 and IGO15342. Run after processing the code in IGO15123 and IGO15342.

**_drug_treatments_** - Contains the Jupyter notebooks to process _KP Slc4a11<sup>MCD/+</sup> Rosa26<sup>mTmG/+</sup>_ tumors lineage traced under treatment with either cisplatin or MRTX1133.  
   1. **_IGO16235_** - Contains the Jupyter notebook to process FACS sorted 17 week _KP Slc4a11<sup>MCD/+</sup> Rosa26<sup>mTmG/+</sup>_ tumors lineage traced with Tamoxifen and treated with either vehicle, cisplatin, or MRTX1133 for 3 weeks.
   2. **_IGO16562_** - Contains the Jupyter notebook to process FACS sorted 17 week _KP Slc4a11<sup>MCD/+</sup> Rosa26<sup>mTmG/+</sup>_ tumors lineage traced with Tamoxifen and treated with either vehicle, cisplatin, or MRTX1133 for 3 weeks.
   3. **_IGO16235\_IGO16562\_combined_** - Contains the Jupyter notebook to concatenate IGO16235 and IGO16562. Run after processing the code in IGO16235 and IGO16562. Generates data for Figure 4.

**_IGO16318-Hopx-MACD-validation_** - Contains the Jupyter notebook to process FACS sorted 16 week _KP Hopx<sup>MACD/+</sup> Hipp11<sup>GGCB/+</sup>_ tumors. Generates data for Extended Data Figures 9.  

**_tracing\_depletion\_analysis_** - Contains the Jupyter notebooks to process depletion cohort (IGO15123\_IGO15342\_combined), traced cohort (IGO15600\_IGO15601\_IGO15771\_IGO16686\_IGO17402\_IGO17543), and untraced control cohort (IGO15488_1_2 and IGO16318) in a uniform manner. Generates data for Fig. 1, and 2, as well as Extended Data Fig. 4, 7, 8, 9, 10, 12, and 17.

**_transplant\_model_** - Contains the Jupyter notebook to concatenate and process FACS sorted IV transplanted _KPfrt Slc4a11<sup>MACD/+</sup>_ cells treated with Saline or DT for 7 days. Generates data for Extended Fig. 14.

## Part 2 - Processing of previously published scRNA-seq data

We downloaded publicly available scRNA-seq data from mouse and human studies across different tissues including colon, skin, prostate, pancreas, and breast. Below is the breakdown of which files were used to analyze the data and the corresponding figures in the publication.

Each dataset was downloaded individually then quality control and analysis was done per dataset as run in the associated python notebook. 

The information was aggregated and compared in the `hpcsQuant-rev.ipynb` file to generate the figures.

We used the `panCancerEnv.yml` to create a conda environment to run the files below.

This Directory generates data for:
- **Figure 5**
- **Extended Data Figures 17 & 18**

### Information Table

| Tissue        | ipynb File                | Gene Signature| Figure                   | PMID     |
|---------------|---------------------------|---------------|--------------------------|----------|
| **Mouse**     |                           |               |                          |          |
| Colon         | mouseColon                | coreHRC       | 5a,e; ED17a              | 36352230 |
| Skin          | mouseSkin                 | lower spike   | 5a,e; ED17a              | 38815020 |
| Prostate      | mouseProstate             | Plasticity    | 5a,b,c,e; ED17a          | 35981096 |
| Pancreas_T    | mousePancreas             | Basal         | 5a,b,c,e; ED17a          | 35952360 |
| Pancreas_B    | mousePancreasB            |               | 5a; ED17a                | 33536616 | 
| Breast        | mouseBreast               |               | 5a; ED17a                | 32840210 |
| Lung          | makeLuadAdata             | HPCS          | 5a,b,c,e; ED17a; ED18a,b | 32707077 |
| Lung          | mouseLung                 | DATP          | 5e; ED17a; ED18b,c       | 32750316 |
| Lung          | mouseLung                 | ADI           | 5e                       | 32678092 |
| Lung          | mouseLung                 | PATS          | 5e                       | 32661339 |
| Skin Injury   | regen_mouseSkin           | wound         | 5e                       | 32187560 | 
|               |                           |               |                          |          |
| **Human**     |                           |               |                          |          |
| Colon         | humanColorectalPelka2021  |               | 5a; ED17a                | 34450029 |
| Skin          | humanSkinJi2020           |               | 5a,c; ED17a              | 32579974 |
| Prostate      | humanProstateDong2020     |               | 5a,c; ED17a              | 33328604 |
| Pancreas      | humanPancreasSteele2020   |               | 5a,c; ED17a              | 34296197 |
| Breast        | humanBreastPal2021        |               | 5a; ED17a                | 33950524 |
| Lung          | humanLungMDA              | KAC           | 5a,c; ED17a,b,c          | 38418883 |
| Lung          | humanLungKim              |               | 5a,c; ED17a              | 32385277 |
| Lung          | humanLungBischoff         |               | 5a,c; ED17a              | 34663877 |
| Lung          | humanLungDost             |               | 5a,c; ED17a              | 32891189 |
| HeadandNeck_C | humanHead-and-Neck        |               | 5a,c; ED17a              | 34921143 |
| HeadandNeck_K | humanHead-and-Neck_K      |               | 5a,c; ED17a              | 32686767 |
| Ovarian       | humanOvarianQ             |               | 5a,c; ED17a              | 35196078 |
| Hematologic(MM) | humanHematologic_L      |               |                          | 33963182 |
| Hematologic(ALL)| humanHematologic        |               |                          | 32415257 |
| Colon Injury  | regen_humanIntestine      | revSSR, revSC | 5e                       | 37162959 | 
|               |                           |               |                          |          |
| **Pan Cancer** |                          |               |                          |          |
| Yanai         |                           | Stress        | ED17a                    | 35931863 |
| Tirosh        |                           | Stress        | 5a                       | 37258682 |



