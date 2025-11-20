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
- **Extended Data Figures 11 & 12**

### Information Table

| Tissue        | ipynb File                | Gene Signature| Figure                   | PMID     |
|---------------|---------------------------|---------------|--------------------------|----------|
| **Mouse**     |                           |               |                          |          |
| Colon         | mouseColon                | coreHRC       | 5c; ED11g; ED12a         | 36352230 |
| Skin          | mouseSkin                 | lower spike   | 5c; ED11g; ED12a         | 38815020 |
| Prostate      | mouseProstate             | Plasticity    | 5a,c; ED11g,h; ED12a     | 35981096 |
| Pancreas_T    | mousePancreas             | Basal         | 5a,c; ED11g,h; ED12a     | 35952360 |
| Pancreas_B    | mousePancreasB            |               | ED11g; ED12a             | 33536616 | 
| Breast        | mouseBreast               |               | ED11g; ED12a             | 32840210 |
| Lung          | makeLuadAdata             | HPCS          | 5a,c; ED11g,h; ED12a,d,e | 32707077 |
| Lung          | mouseLung                 | DATP          | 5c; ED12a,d,e            | 32750316 |
| Lung          | mouseLung                 | ADI           | 5c                       | 32678092 |
| Lung          | mouseLung                 | PATS          | 5c                       | 32661339 |
| Skin Injury   | regen_mouseSkin           | wound         | 5c                       | 32187560 | 
|               |                           |               |                          |          |
| **Human**     |                           |               |                          |          |
| Colon         | humanColorectalPelka2021  |               | ED11g; ED12a             | 34450029 |
| Skin          | humanSkinJi2020           |               | 5a; ED11g; ED12a         | 32579974 |
| Prostate      | humanProstateDong2020     |               | 5a; ED11g; ED12a         | 33328604 |
| Pancreas      | humanPancreasSteele2020   |               | 5a; ED11g; ED12a         | 34296197 |
| Breast        | humanBreastPal2021        |               | ED11g; ED12a             | 33950524 |
| Lung          | humanLungMDA              | KAC           | 5a; ED11g; ED12a-c       | 38418883 |
| Lung          | humanLungKim              |               | 5a; ED11g; ED12a         | 32385277 |
| Lung          | humanLungBischoff         |               | 5a; ED11g; ED12a         | 34663877 |
| Lung          | humanLungDost             |               | 5a; ED11g; ED12a         | 32891189 |
| HeadandNeck_C | humanHead-and-Neck        |               | 5a; ED11g; ED12a         | 34921143 |
| HeadandNeck_K | humanHead-and-Neck_K      |               | 5a; ED11g; ED12a         | 32686767 |
| Ovarian       | humanOvarianQ             |               | 5a; ED11g; ED12a         | 35196078 |
| Hematologic(MM) | humanHematologic_L      |               |                          | 33963182 |
| Hematologic(ALL)| humanHematologic        |               |                          | 32415257 |
| Colon Injury  | regen_humanIntestine      | revSSR, revSC | 5c                       | 37162959 | 
|               |                           |               |                          |          |
| **Pan Cancer** |                          |               |                          |          |
| Tirosh        |                           | Stress        | ED11g                    | 37258682 |
| Yanai         |                           | Stress        | ED12a                    | 35931863 |
