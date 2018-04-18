---
layout: post
title:  "Patent Analysis Project"
date:   2018-04-18
excerpt: "Click Read More to view my R Notebook showing analysis of patent data in collaboration with Legal Analytics"
project: true
feature: http://jamocko.github.io/assets/img/LegalAnalytics.png
tag:
- projects
- R notebook
comments: true
---

## Overview
<b>Patent Analysis</b> is one of my R notebooks containing data exploration and statistical analysis for a project analyzing PTAB patent data to identify potential predictors of which patents will succeed or fail in becoming institutionalized.  

<div markdown="0"><a href="http://juliemocko.com/notebooks/" class="btn btn-info">View R Notebook - COMING SOON</a></div> 

## Background  
*Please note that the data have been altered, and the results are reported in a vague fashion for the purposes of display in my portfolio, as the data are sensitive.*

The **patent analysis project** was done as a collaboration between myself (as a freelance data scientist) and David Andrews, JD of [Legal Analytics](http://analytics.legal/).  Below is a summary of my findings for this project:
<hr>

## Goal  
The goal of this project was to explore the PTAB data and determine whether any measures could be used to aid in the prediction of the patent outcome.  We have found that none of the measures in the data set were good predictors of whether or not a patent became “institutionalized”.

## Methods  
In our analysis, the outcome was divided into two possibilities.  A patent receiving a “Not Institutionalized – Merit” decision was considered a negative outcome.  A patent receiving any other decision was considered a positive outcome.  We also excluded the following outcomes from the analysis: Adverse Judgment, Not Institutionalized – Procedural, Pending, Procedural Termination, and Settlement.  Only the IPR cases were considered in the analysis.

The following measures were analyzed:

* PTAB tech center
* Entity
* Industry
* Claim score
* Patent processing time
* Patent year
* Patent citations
* Patent description length
* CPC group

A logistic regression predictive mathematical model was used to determine which, if any, of these measures could be used to predict whether or not future patents become institutionalized.

## Results  
None of the measures analyzed were strongly associated with whether or not a patents was institutionalized.  According to the model, the following measures showed a slight association with the outcome.  Please note that the following associations describe a general trend across all of the data, and will not necessarily imply that any given patent will show this relationship.

**Type of industry:**
Patents originating from “tech” and “other” industries were more likely to have a positive outcome (institutionalized) than patents from the “medical” industry.  

**Claim score:**  
Patents with higher claim scores had a slight tendency towards having a positive outcome.

**Patent description length:**  
Patents with greater description detail length had a slight tendency towards having a positive outcome.

Despite the slight association between these measures and the outcome, the predictive model revealed that none of these measures are good predictors.  

Using the PTAB data set, the model was able to correctly predict the outcomes of 64% of the patents, giving an incorrect prediction 36% of the time (36% misclassification rate).  If one were to predict that all patents would have a positive outcome without taking into account any information about the patent, they would correctly predict the outcomes of 63% of the patents (37% misclassification rate).  That the predictive model using the PTAB data only out-performs the prediction that “all patents will succeed” by 1%, indicates that none of the metrics in this data set are good predictors of whether a patent will be institutionalized. 
