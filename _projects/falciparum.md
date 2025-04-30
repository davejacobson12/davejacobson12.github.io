---
layout: page
title: Monitoring Antimalarial Drug Resistance
description: Characterizing P. falciparum genomes and high-profile case investigations
img: /assets/img/incidence-of-malaria.png
importance: 6
category: Nationwide Parasitic Disease Surveillance
---

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/aac.01203-24.f003.jpg ' | relative_url }}" alt="" title="example image"/>
    </div>
</div>
---

### Background 
The United States sees about 1,000 to 2,000 cases of *P. falciparum* malaria in travelers returning from malaria endemic countries, primarily in sub-Saharan Africa. Since 2014, CDC has requested that State Public Health Labs submit blood samples from these cases in order for CDC to identify antimalarial drug resistance across 6 genes. When combined with antimalarial drug efficacy studies performed in endemic regions, information on antimalarial drug resistance in returning travelers can inform guidance on which antimalarial prophylaxis are most likely to be effective and thus be recommended to be prospective travelers. While informative, the sequencing data was generated from 6 short amplicons (1 for each gene) and thus limits the data that can be gleaned from these samples.

My team's goal was to transition CDC from using a amplicon-based approach to a whole-genome based approach (i.e., selective whole-genome amplificatio, or sWGA) for *P. falciparum* surveillance. The sWGA approach allows CDC to capture the full length of the original 6 genes, plus potential novel genes/mechanisms of antimalarial resistance, as well as facilitating genome-wide comparisons that can inform public health researchs on *P. falciparum* genomic characteristics that are hidden when only using amplicon data.

### Analysis
I worked with teammembers to write a bioinformatic workflow that analyzes sWGA data to call antimalarial drug resistance SNPs, identify complexity of infection (COI), predict geographic origin, detect HRP2/3 deletions, and facilitates clustering of closely related parasites. By benchmarking and validating the antimalarial drug resistance SNP calling of the sWGA workflow, we were able to continue our main goal of detecting drug resistance in the primary 6 genes, while adding the workflow componants listed above, which were not possible with amplicon data. 

COI detection, HRP2/3 deletion, and geographic origin are all useful analyses to more fully describe the *P. falciparum* parasites making returning travelers sick. It allows us to perform a more complete malaria genomic surveillance. Likewise, were able to add the *Pfcoronin* gene to our antimalarial drug resistance detection workflow and more genes were in the process of being added to the workflow when I left CDC. Using sWGA data also facilitates assessing copy number variation, not just SNPs, in drug resistance which again expands CDC's understanding of malaria in returning travelers.

### Findings
Through genetic clustering of sWGA data, we were able to link cases together in a presumed hospital-acquired malaria case. Additionally, we were able to confirm that a laboratorian in an independent lab likely contracted malaria from a common control *P. falciparum* strain used in labs across the world. 

Our sWGA drug resistance workflow called 99% of the same drug resistance SNPs as the amplicon workflow. The discrepencies were identified in edge cases for calling mutant vs wildtype in mixed infections, where change of a few reads one way or the other caused a different genotype to called between the amplicon and sWGA workflows.

Our geographic prediction assay was also over 99% accurate at placing the parasites genome in the geographic region where the infection was acquired. This is valuable information in the 10-25% of cases where travel history is not provided to CDC, since we can use the geographic prediction data to inform whether the *P. falciparum* parasite has drug resistance mutations that are consisten with its geographic region, or if known mutations are spreading into new geographic regions.

### My Role
- Study Design: Development of geographic prediction panels, identify genes for novel antimalarial resistance analysis
- Analysis: Bioinformatic analysis (QC, mapping, SNP calling, indel analysis), statistical analysis (clustering, geographic prediction, complexity of infection, drug resistance interpretation)
- Communication: Presentations to leadership, CDC epidemiologists, State Public Health Department epidemiologists
- Publications: supporting author, figure generation, manuscript draft

### Publications
White J. L., Ridpath A. D., Guzzardi E., Smith K., Slavinski S., Antwi M., Lee E., Barrett K., Southwick K. L., Gayen S., Quinn M. J., Mace
K. E., Williams S., Raphael B., **Jacobson, D. K.**, Barratt J. L. N., McElroy P., Antenucci S., Clemons B. M., McKinney K. and Backenson
B. (In Preparation). Case Report and Epidemiological Investigation of Healthcare-associated Plasmodium falciparum Malaria
Transmission in Westchester County, New York- 2023

Pierre-Louis, E., Kelley, J., Patel, D., Carlson, C., Talundzic, E., **Jacobson, D. K.**, and Barratt, J. L.N. (2024). Geo-classification of
drug-resistant travel-associated Plasmodium falciparum using Pfs47 and Pfcpmp gene sequences (USA, 2018–2021). Antimicrobial
Agents and Chemotherapy 68(12), e01203-24.