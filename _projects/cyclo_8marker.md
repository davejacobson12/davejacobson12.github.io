---
layout: page
title: Foodborne Disease Outbreak Detection
description: Identifying and reporting Cyclospora foodborne outbreaks
img: /assets/img/1-s2.0-S2667114X2300033X-ga1_lrg.jpg 
importance: 4
category: Nationwide Parasitic Disease Surveillance
---

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/1-s2.0-S2667114X2300033X-gr2.jpg' | relative_url }}" alt="" title="example image"/>
    </div>
</div>
---

### Background 
Cyclosporiasis is a foodborne illness that afflicts a couple thousands of Americans every year, primarily in btween the months of May and September. The disease is caused by consuming produce or water contaminated with a sporulated (and thus infectious) *Cyclospora* parasites. CDC developed a genotyping approach using 8 markers spread across *Cyclospora*'s 45 megabase genome and this approach, when paired with the appropriate bioinformatic and clustering algorithms, has proving to be highly accurate at identifying clusters of genetically related parasites. Our lab team communicates the resulting genetic clusters and their temporal relationships to epidemiologists, who try to identify common food exposures and likely sources for distinct outbreaks.

My initial role was to modernize and optimize CDC's *Cyclospora* genotyping workflow by transition the bioinformatic pipeline from running off-premises on an individual MacBook Pro to a containerized pipeline running on CDC's Scientific Computing (SciComp) high-perfomance computing environment. From there, I worked on optimizing the clustering algorithms and improve workflows to link genetic sequencing data to lab and epidemiologic data. Finally, had a lead role in interfacing with federal and state partners across the United States to manage the surveillance program, from sample submission, to data generation troubleshooting, to generating informative reports that influence public health actions.

Outside of the typical domestic surveillance, we were involved in working with FDA to identify new genoypting markers that could provide improved genoytping resolution and facilitate linking *Cyclospora* genotypes found in human samples (which is CDC's purview) to *Cyclospora* genotypes found in produce (which is FDA's purview). This project was underway when I left CDC.

### Analysis
I translated the *Cyclospora* genotyping workflows from BASH into Nextflow and containerized workflows using Singularity. The complexity of the workflows is difficult to get across in text, and thus I encourage readers to examine the workflows on my [GitHub page](https://github.com/davejacobson12/Portfolio/tree/main/Bioinformatic_Pipelines). The goal for these workflows is to take clean amplicon reads from each of the 8 markers and cut them into ~100bp chunks to identify repeated/novel haplotypes at each part of each marker. The shared haploytpes between each pair of samples is used as a the basis to calculate sample similarity and cluster genetically similar specimens together.

After bioinformatically processing samples, I wrote workflows to link bioinformatic, lab, and epi data into various reports. An example of the type of reports we shared with our state partners can be found on my projects page, or take this direct [link](https://davejacobson12.github.io/cyclospora_genotyping_report/).

### Findings
Over the four cyclosporiasis genotyping seasons I was a part of, we identified 12 distinct outbreaks where bioinformatic data was used to confirm epidemiologic outbreaks. There were a large number of other genetic clusters that were identified during this time period; however, there was not sufficient epidemiologic data to identify a common source for those outbreaks. 

Initial results from working with FDA to identify new genotyping markers appeared promising for multiple reasons. The new genoytping markers were able to identify a handful of clusters that were not identified using the 8 marker approach. At the same time, the majority of clusters identified with the new kit matched the clusters identified with the 8 markers, indicating the 8 genotyping markers and analysis workflow is still useful if the larger genotyping kit proves too difficult to adopt for regular molecular surveillance.

### My Role
- Study Design: Identify additional genotyping markers, design sample/sequence data submission
- Study Management: Manage sample databases, regular communication with state and federal partners for sample submission and reporting
- Analysis: Bioinformatic analysis (QC, mapping, workflow development), statistical analysis (clustering, temporal linkages, link to epi data)
- Communication: Presentations to leadership, CDC epidemiologists, State Public Health Department epidemiologists
- Publications: lead and supporting author, figure generation, manuscript draft

### Publications
Peterson, A. C., **Jacobson, D. K.**, Richins, T., Barratt, J. L.N., and Qvarnstrom, Y. (Accepted). Assessing the sequencing success and analytical specificity of a targeted amplicon deep sequencing workflow for genotyping the foodborne parasite Cyclospora. Journal
of Clinical Microbiology.

Shen, J., Cama, V. A., **Jacobson, D. K.**, Barratt, J. L.N., and Straily, A. (2025). Cyclospora Genotypic Variations and Associated
Epidemiologic Characteristics, United States, 2018–2021. Emerging Infectious Diseases 31(2), 256.

Leonard, S. R., Mammel, M. K., Almeria, S., Gebru, S. T., **Jacobson, D. K.**, Peterson, A. C., Barratt, J. L.N., and Musser, S. M. (2024). Evaluation of the Increased Genetic Resolution and Utility for Source Tracking of a Recently Developed Method for Genotyping
Cyclospora cayetanensis. Microorganisms 12(5), 848.

Kahler, A. M., Hofstetter, J., Arrowood, M., Peterson, A. C., **Jacobson, D. K.**, Barratt, J., da Silva, A. L. B. R., Rodrigues, C., and Mattioli, M. C. (2024). Sources and prevalence of Cyclospora cayetanensis in southeastern US growing environments. Journal of
food protection 87(7), 100309.

**Jacobson, D. K.**, and Barratt, J. L.N. (2023). Optimizing hierarchical tree dissection parameters using historic epidemiologic data as ‘ground truth’. Plos one 18(2), e0282154.

**Jacobson, D. K.**, Peterson, A. C., Qvarnstrom, Y., and Barratt, J. L.N. (2023). Novel insights on the genetic population structure of human-infecting Cyclospora spp. and evidence for rapid subtype selection among isolates from the USA. Current Research in
Parasitology and Vector-Borne Diseases 4(), 100145.

Ahart, L., **Jacobson, D. K.**, Rice, M., Richins, T., Peterson, A. C., Zheng, Y., Barratt, J. L.N., Cama, V., Qvarnstrom, Y., Montgomery, S., and Straily A. (2023). Retrospective evaluation of an integrated molecular-epidemiological approach to cyclosporiasis outbreak investigations–United States, 2021. Epidemiology and Infection 151(), e131.

Peterson, A. C., Richins, T., Houghton, K., Mishina, M., Sharma, S., Sambhara, S., **Jacobson, D. K.**, Qvarnstrom, Y., and Cama, V.
(2023). The limit of detection of the BioFire® FilmArray® gastrointestinal panel for the foodborne parasite Cyclospora cayetanensis.
Diagnostic Microbiology and Infectious Disease 107(2), 116030.

**Jacobson, D. K.**, Low, R., Plucinski, M. M., and Barratt, J. L.N. (2023). An improved framework for detecting discrete
epidemiologically meaningful partitions in hierarchically clustered genetic data. Bioinformatics Advances 3(1), vbad118.

**Jacobson, D. K.**, Zheng, Y., Plucinski, M. M., Qvarnstrom, Y., and Barratt, J. L. N. (2022). Evaluation of various distance computation methods for construction of haplotype-based phylogenies from large MLST datasets. Molecular phylogenetics and evolution 177(), 107608.