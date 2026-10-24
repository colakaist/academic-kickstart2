---
title: "Active learning enables long-timescale simulations of diluent-modulated ionic liquid electrolytes"
authors: [A. Mariam, S. Choe]
#- schoe

date: "2026-10-21"
doi: ""
volume: ""
pages: ""

# Schedule page publish date (NOT publication's date).
#publishDate: ""

# Category
# Legend:  Theoretical Physics; Biophysics; Condensed Matter Physics
categories: ["Condensed Matter Physics"]

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["1"]

# Publication name and optional abbreviated publication name.
publication: "2026 KPS Fall Meeting (10/20-10/23, Jeju)"
publication_short: ""

abstract: "The rational design of ionic liquid electrolytes (ILs) is hindered by a persistent trade-off in molecular simulation: classical force fields offer computational efficiency but often require laborious, system-specific parameterization and may exhibit limited transferability across chemical environments, whereas first-principles methods provide high accuracy but cannot readily access the length and time scales required to capture the slow, collective dynamics governing ion transport. Machine-learning interatomic potentials offer a promising route to bridge this gap by approaching density functional theory (DFT) accuracy at substantially reduced computational cost. Here, we demonstrate that a moment tensor potential (MTP), trained on DFT reference data through on-the-fly active learning, enables accurate and computationally efficient simulations of diluent-modulated ILs over extended time scales. By selectively incorporating informative configurations into the training set, active learning substantially reduces the amount of reference data required while maintaining accuracy across a broad range of diluent concentrations. The resulting MTP reproduces key structural and thermodynamic properties, including lattice parameters and densities, in close agreement with DFT calculations. More importantly, long-timescale simulations capture the concentration-dependent evolution of solvation structures and ionic transport upon dilution, consistent with previous computational studies and experimental measurements. The MTP thus reproduces not only equilibrium properties but also the concentration-dependent trends characteristic of locally concentrated ionic liquids, where changes in local solvation environments strongly influence ion-transport pathways. These results demonstrate that actively learned MTPs can combine first-principles-level accuracy with transferability across composition and access to the time and length scales required to describe ion transport. This framework provides a practical route toward predictive, first-principles-quality simulations for the rational design of ionic liquid electrolytes."

# Summary. An optional shortened abstract.
#summary: []

#tags:
#- Source Themes

featured: false

# links:
# - name: ""
#   url: ""
#url_pdf: http://arxiv.org/pdf/1512.04133v1
url_code: ''
url_dataset: ''
url_poster: ''
url_project: ''
url_slides: ''
#url_source: 'https://papers.ssrn.com/sol3/papers.cfm?abstract_id=4539335'
url_video: ''

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
#image:
#  caption: 'Image credit: [**Unsplash**](https://unsplash.com/photos/jdD8gXaTZsc)'
#  focal_point: ""
#  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g.  MD(Materials Design)  
#   Otherwise, set `projects: []`.
projects: [MD]

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
#slides: example
---



