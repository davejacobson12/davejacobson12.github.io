---
layout: page
title: Tracking Domestic Malaria Cases
description: Identifying locally transmitted P. vivax in the U.S.
img: /assets/img/vivax_image.png
importance: 5
category: Nationwide Parasitic Disease Surveillance
---

<!-- <div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/scfa.jpg' | relative_url }}" alt="" title="example image"/>
    </div>
</div> -->
---

### Background
Malaria was considered endemic in the southern United States into the early 1950s but concerted efforts in vector control led to eradication. Local transmission of malaria has been rare, with the most recent locally acquired malaria cases occurring in 2003; however, health departments reported likely cases of locally acquired malaria in Florida and Texas in 2023. Each of these cases were verified to be *Plasmodium vivax* and CDC did not have a method for genetically comparing *P. vivax* cases to each other. Our team was tasked with creating a genotyping tool that would allow CDC to determine genetic relatedness amongst the locally acquired cases. I worked closely with my supervisor and laboratorians to perform thorough literature searches to identify appropriate genotyping markers and develop a bioinformatic pipeline to urgently address questions about parasite relatedness for these cases

### Analyses
Our team created an Illumina AmpliSeq panel based on existing literature and incorporating additional target genes recommended by senior leadership. I wrote bioinformatic pipelines to process the sequencing data through a clustering pipeline that was originally developed for detecting foodborne outbreak clusters of *Cyclospora*. In addition, I optimized machine learning algorithms that allowed us to predict the geographic origin of all *P. vivax* parasites that we genotyped. Finally, I was heavily involved in building a reference population from published data and from CDC's sample archive to present a full picture of how genetic data from the locally acquired cases compares to other *P. vivax* genomes.

### Findings 
Our clustering algorithm determined that cases locally acquired in Florida in 2023 were genetically different from the cases acquired in Texas. Likewise, the 2023 Florida cases were distinct from the 2003 Florida cases, suggesting that the 2003 Florida, 2023 Texas, and 2023 Florida outbreaks were all the result of independent introductions. All of these cases had geographic signatures that aligned with a Central / South American origin.

Interestingly, 2023 saw a large number of imported *P. vivax* cases that were unrelated to the locally acquired cases. These imported cases were linked to individuals who had travelled abroad but reported malaria symptoms after returning to the United States. Our genotyping results indicated there were large, distinct clusters associated with the imported cases. Further analysis of whole-genome sequencing data completed in the days before I left CDC indicated that these cases match a geographic signature from Panama, and not South America. More analysis is required to further flesh out the implications from these findings.

### My Role
- Study Design: Genotyping panel design, bioinformatic pipeline development, machine learning algorithm optimization, selecting samples to analyze
- Study Management: Manage sample databases
- Analysis: Bioinformatic analysis (QC, mapping, SNP calling), statistical analysis (clustering, geographic prediction)
- Communication: Presentations to leadership, CDC epidemiologists, State Public Health Department epidemiologists
- Publication: supporting author, figure generation


### Publications

Barratt, J. L.N., **Jacobson, D. K**, Pierre-Louis, E., Bajic, M., Kelley, J., Patel, D. S., Goldman, I., Zhou, Z., Shi, Y. P., Ridpath, A., Mace, K., Carlson, C., Sutcliffe, A., Butler, Q., Morrison, A., Stanek, D., Tomson, K., Blackmore, B., Cannons, A., Rollo, S., Wang, C., Tuladhar, R., Clemons, B., Antenucci, S., Mergen, K., White, J., Antwi, M., Rothfeldt, L., Lazenby, K., Hedges, S., Shray, J., Courtney, A., Boyanton, B., Qvarnstrom, Y., Freeman, M., and Raphael, B. (Under Review). Genetic characterization of Plasmodium vivax linked to autochthonous malaria transmission in the US (2023) using Illumina AmpliSeq technology: a genetic epidemiology study. Lancet Regional Health - Americas.