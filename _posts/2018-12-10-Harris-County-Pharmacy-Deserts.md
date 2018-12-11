---
layout: post
title:  "[R] Harris County Pharmacy Deserts Project"
date:   2018-12-10
excerpt: "Click Read More to view my R Notebook showing a visualization of closest pharmacy distances by block group in Harris County"
project: true
feature: 
tag:
- projects
- R notebook
comments: true
---

## Overview
<b>Harris County Pharmacy Deserts</b> is one of my R notebooks visualizing pharmacy distances by block group in Harris County, with highlighting of regions with vulnerable populations.  

<div markdown="0"><a href="http://juliemocko.com/notebooks/harris-county-pharmacy-deserts/" class="btn btn-info">View R Notebook</a></div> 

## Background
The purpose of this notebook is to identify pharmacy deserts in Harris county.

**Purpose:** Accessibility to a pharmacy is an important facilitator of overall health, and is critical to ensure proper utilization of medications and adequate delivery of healthcase services. Community pharmacies offer a wide spectrum of services including dispensing medications, patient counselling, screening tests, immunization services, wellness programs, and education programs. Unlike many other healthcare settings, community pharmacies offer greater accessibility, with their extended hours of operation, availability of home delivery of medications, and no need to schedule an appointment for services.

However, not everyone has equal access to community pharmacies. Similar to “food deserts”, coined by the USDA, there exist “pharmacy deserts”, or geographic areas which lack access to a nearby pharmacy and where pharmacy services are scarece or difficult to obtain. Prominent public health researcher Dima M. Qato has defined pharmacy deserts in urban areas as regions where there is no pharmacy within one mile.

**Methods:** A dataset of licensed pharmacies in Texas was obtained from the Texas State Board of Pharmacy website. For the purposes of this analysis, pharmacies were limited to “Community Pharmacies” with active licenses. Other types of pharmacies, including those that only provide mail-order prescriptions, were excluded.

Census blocks are colored by closest distance from the center of the block to a pharmacy. Distances of greater than 1 mile have been used to denote pharmacy deserts in urban areas, however, for vulnerable populations (elderly, ill, families with young children, or people below the poverty line), even smaller distances can prove to be prohibitive.

**Next Steps:** Quantification and analysis of pharmacy deserts in Harris County and associated demographic information from desert regions.  

<div markdown="0"><a href="http://juliemocko.com/notebooks/harris-county-pharmacy-deserts/map/" class="btn btn-info">View Interactive Map</a></div>
