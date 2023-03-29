---
layout: page
title: Cell type labeling
description: Evaluation of 26 cell annotation algorithms for single cell RNA sequencing data
img: assets/img/labeling.png
importance: 2
category: research
---

Identifying the population of cells in the tumor microenvironment is the first step to study a single cell RNA sequencing (scRNA-seq) dataset. In this project, we reviewed and evaluated 26 (19 supervised and 7 unsupervised) state-of-the-art algorithms for annotating the scRNA-seq data.

The performance of the 26 algorithms are sumarrized in the following two figures. Details of our analysis can be found in our [paper](https://academic.oup.com/bib/article/24/1/bbac561/6965910) published in <i>Briefings in Bioinformatics<i>.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/Figure_2.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Performance and running time summary of cell type prediction methods across eight cancer datasets.
</div>




<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.html path="assets/img/performance.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Performance of the 26 algorithms.
</div>

