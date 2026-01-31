# Sesion 3: 31 de enero de 2026

Abramos un documento Rmd

```
title: "Mi fabuloso título"
author: "Mi nombre"
date: "`r Sys.Date()`"
output: 
  html_document:
    theme: cerulean
```
Intenten cambiar el `theme` por alguna(s) de estás opciones

+ journal
+ flatly
+ united
+ cosmo
+ simplex

```
title: "Mí fabuloso título"
author: "Mi nombre"
date: "`r Sys.Date()`"
output: 
  html_document:
    theme: cosmo
    toc: yes
    toc_float:
      collapsed: true
```

```
output: 
  html_document:
    theme: cerulean
    toc: yes
    toc_float:
      collapsed: true
```

```
output: 
  html_document:
    theme: lumen
    toc: yes
    toc_float:
      collapsed: true
```

```{r}
library(rmdformats)
library(prettydoc)
library(hrbrthemes)
library(tint)
library(tufte)
```

```
output: 
  prettydoc::html_pretty:
    theme: hpstr
```

```
output: 
  prettydoc::html_pretty:
    theme: cayman
    toc: yes
```

```
output: 
  rmdformats::readthedown
```
