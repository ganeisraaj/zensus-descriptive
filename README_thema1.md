# Thema 1 — Descriptive Analysis of Education and Employment in German Districts
**Deskriptive Analyse von Bildung und Erwerbstätigkeit in deutschen Kreisen**

**Technische Universität Dortmund | Department of Statistics | SoSe 2026**
Supervised by Prof. Dr. Katja Ickstadt, JProf. Dr. Nils Weitzel, Dr. Zeyu Ding
Author: Ganeisraaj Kathiravan | Group partner: Jakub Marczat

---

## Overview / Überblick

This project uses the 2022 German Census (Zensus 2022) to explore education and labour market outcomes across 400 German districts and independent cities. The central question is whether structural differences in qualification and employment rates between East and West Germany persist more than three decades after reunification, and which district-level variables are most strongly associated with unemployment.

Dieses Projekt nutzt den Zensus 2022, um Bildungs- und Arbeitsmarktvariablen in 400 deutschen Kreisen und kreisfreien Städten zu untersuchen. Die zentrale Frage ist, ob strukturelle Unterschiede zwischen Ost- und Westdeutschland mehr als drei Jahrzehnte nach der Wiedervereinigung fortbestehen und welche Variablen auf Kreisebene am stärksten mit der Erwerbslosenquote assoziiert sind.

---

## Data / Daten

| | |
|---|---|
| **Source** | Statistisches Bundesamt (Destatis), Zensus 2022 |
| **Reference date** | 15 May 2022 |
| **Unit of observation** | 400 Kreise und kreisfreie Städte |
| **Key variables** | Abitur rate, unemployment rate, employment rate, economic inactivity rate, gender gaps, population |

---

## Methods / Methoden

- Descriptive statistics (mean, median, standard deviation, IQR)
- Outlier identification via the 1.5 × IQR rule
- Univariate distribution analysis: histograms and boxplots, separately for East and West Germany
- Pairwise scatterplots coloured by East/West status
- Pearson correlation analysis and correlation plot (`psych::cor.plot`)
- Systematic East–West comparison

---

├── report.pdf        # English-language report
├── analysis.R        # R script (data cleaning, visualisation, analysis)
└── data/
    ├── zensus2022_wide.csv
    └── zensus2022_long.csv
```

---

## Software

R 4.5.x · `tidyverse` · `ggplot2` · `psych` · `patchwork`
