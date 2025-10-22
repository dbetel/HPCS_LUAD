# HPCS_LUAD
Code base for high-plasticity cell state in lung adenocarcinoma study by Chan*, Pan* et. al. 

_Requirements_: SCANPY, AnnData, Scipy

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


