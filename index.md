---
title       : Shiny App
subtitle    : Fluxomic Analysis
author      : 
job         : https://kappacoo.shinyapps.io/App-1/
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
mode        : selfcontained # {standalone, draft}
--- 

## Fluxomic Analysis
### The Background: Metabolomics
I work in the field of metabolomics. Our main task is trying to understand how metabolism changes in response to different conditions (i.e. changes in diet) by measuring metabolites (glucose, ATP, lactate, etc.). 

In our case, we measure metabolites my mass spectrometry. Each metabolite has a known mass that we use to identify it. We often combine mass spectrometry with some column separation technique (gas chromatography or liquid chromatography) which helps us separate compounds of similar masses. 

---

### The Background: Fluxomics

To better understand metabolism of a specific compound (let's say glucose), we introduce stable isotopes. For every stable isotope (Carbon 13, C13) that replaces the more prevalent isotope (C12), we get a 1 dalton shift in mass, which we denote as M+1. 

That means, if each of the carbons of glucose (a 6-carbon molecule) are replaced with C13, then we will observe M+6 glucose. 

Measuring this mass shift in many different metabolites is termed <b>"Fluxomics"</b>. 

--- 

### The Problem
At the start of my work, most of the analysis was done in Excel.

* Pros: Easy to understand and easy to share with others.  
* Cons: Hours of formatting graphs.

### The Solution
Learning R and making a function that plots the graphs.

* Pros: Fast; all the graphs I want in less than 1 min.  
* Cons: Very few of my colleagues know R; my useful tool was not getting used (except by me).


<br/>
#### <b>Conclusion: I needed a tool that could be easily shared with my colleagues.</b>


--- 

## The Shiny App: Fluxomics Analysis

This shiny app is fairly simple - it plots graphs and lets you download them. 

Some important features:
- User can load in their data. 
- Metabolites and their various isotopes (M+1, etc) can be graphed together. 
- Automatic mean and standard error (error bars) for each comparison group.
- Various ways to look at the data (%, relative peak area, single isotopes, merged isotopes).
- Fast, interactive, and the user doesn't need to know R!

<br/>
# https://kappacoo.shinyapps.io/App-1/ 
