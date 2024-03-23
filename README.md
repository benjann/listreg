# listreg
Stata module for the analysis of list experiments using linear regression

`listreg` fits a linear model to data from a list experiment
(a.k.a. item count technique) or to data collected by the item-sum technique. 
Single-list and double-list designs are supported.

Stata version 14 or newer is required.

---

Installation from SSC:

    . ssc install listreg, replace

Installation from GitHub:

    . net from https://raw.githubusercontent.com/benjann/listreg/main/
    . net install listreg, replace

---

Main changes:

    23mar2024 (version 1.0.2)
    - in the double-list design the default now is to use all available observations
      for each list and not restrict the analysis to the common sample; specify
      option -listwise- (or -casewise-) for old behavior
    - option -aequations- to include auxiliary equations (i.e. the shortlist models)
      in the results
    - option -nodf- renamed to -nodfr-

    14mar2024 (version 1.0.1)
    - some changes to handling of tvar

    14mar2024 (version 1.0.0)
    - released on GitHub
