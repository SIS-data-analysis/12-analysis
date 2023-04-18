# April 11/18: Analysis
### Description, inference, and linear association

Step beyond data wrangling and visualization and into the world of statistical analysis. Can we use the data we cleaned, collected, and described to answer empirical questions? Part 1 covers analysis of numeric variables: summary stats, difference of means, ANOVA, and linear regression. Part 2 will cover interaction effects, categorical predictors, tabular analysis, and transformations.

## Prep for class
- In case you want a basic refresher, see Chs 5-7 of the [SIS 600 Survival Guide](https://austin-hart-pols.github.io/SurvivalGuide/)
- See also Ch 7 of Winston Chang's [Cookbook for R](http://www.cookbook-r.com/)
- Data for class [coming soon]
- [`posterdown` package](https://github.com/brentthorne/posterdown) and [lengthier example](https://shilaan.rbind.io/post/academic-conference-posters-using-posterdown/) of using it

Installing first time:

```
# Installing posterdown and some key dependencies
  install.packages('posterdown')
  
# Check on tinytex
  tinytex::is_tinytex() # if TRUE, you're all done! if false, proceed to next step
    install.packages('tinytex') # if you haven't already
    tinytex::install_tinytex()
      tinytex::is_tinytex() # if TRUE, all done
```

Consider also a YAML for the `posterdown` option:

```
---
title: '**Title of my paper or project**'
author:
  - name: '**My Name**'
    affil: 1
    main: true
    twitter: myname123 
    email: myname@myhouse
affiliation:
  - num: 1
    address: Department of things, My Uni
main_findings:
  - "I have some things to say"
  - "I found **really important** things, and you should cite me!"
main_topsize: 0.2 
main_bottomsize: 0.1
primary_colour: "#0063B2FF"
secondary_colour: "#9CC3D5FF"
accent_colour: "#cc0000"
output: 
  posterdown::posterdown_betterport:
    self_contained: false
    pandoc_args: --mathjax
    number_sections: false
bibliography: packages.bib
link-citations: true
---
```

## Assessment
- Poster: submit electronically via Canvas April 21.
