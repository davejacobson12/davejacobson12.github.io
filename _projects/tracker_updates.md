---
layout: page
title: ETL Workflows for Internal Sample Tracking
description: Cleaning, merging, maintaining genomic surveillance databases
img: /assets/img/big-data-7216839_1280.png 
importance: 7
category: ETL Workflows and Report Examples
---

### Background
CDC receives and/or generates DNA sequencing data for about 1,500 Cyclospora cases from about 30 states every year, with over 98% of submissions coming between June 1st and September 30th. My team's goal was to identify genetic clusters and report these genetic clusters to epidemiologists, who can then link genetic clusters to known outbreaks and/or identify common foods consumed by the cases in each genetic cluster. The end result would be sets of multistate outbreak clusters that were confirmed by genetic and epidemologic data; the clusters were used by FDA to identify the farm/firm associated with the implicated produce. The complex, high-stakes nature of these investigations meant it was paramount to keep diligent records of each sample submitted, how it was processed, and its genotyping results.

In my last 1.5 years at CDC, I joined a newly created Domestic Surveillance Team that incorporated *Cyclospora* and *Malaria* genomic surveillance as part of the same team. I lead efforts to work closely with malaria lab staff and epidemiologists to create workflows that mimicked our *Cyclospora* workflows, albeit with a number of differences to account for variation in sample processing and epidemiological needs.

### Analysis

I wrote workflows in R and python to extract, transform, and load data from a variety of sources and maintained our historical genotyping databases for *Cyclospora* and *Malaria*. The datasources are as follows: DNA sequence data (FASTQ files), DNA/Sample submission forms (excel format, termed the GFAT), laboratory results (csv/text format), genotyping results (csv/text format), epidemiologic data (csv format), and internal laboratory master sheets (excel format). These data sources were linked by a few different keys: submission forms, epidemiologic data, and laboratory master sheets were linked by a Case ID; laboratory results and laboratory master sheets were linked by a Sample ID;DNA sequence data, submission forms, genotyping results, and laboratory master sheets were linked by a Sequence ID. 

The workflows I wrote performed a variety of checks to ensure the correct data was being merged and cleaned. Additionally, the scripts would automatically update and format our master spreadsheets using the most recently generated data, allowing lab staff to focus lab work and not timely data entry. These scripts decreased data entry errors substantially (up to 80%) and saved roughly 5-10 hours a week across all lab staff, depending on how many samples were being processed.

I also spearhead the implementation of a universal sample naming convention to eliminate previous issues related to sample naming and data entry errors.

### My Role
Project Conception: Build malaria ETL workflows from scratch, create sample naming convention, create submission forms
Technical Duties: Write R and python code for ETL workflows, write python code to automate master sheet formatting for lab staff, troubleshooting when data entry inconsistencies generate error codes in workflow
Communication: Inform partners of sample/sequence data submission and receipt, train staff and partners on their responsibilities