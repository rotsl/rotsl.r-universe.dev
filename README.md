# Take package. Use package. Happy.

Big cave for packages made by [**rotsl**](https://github.com/rotsl).

---

## Status

[![packages status badge](https://rotsl.r-universe.dev/badges/\:packages)](https://rotsl.r-universe.dev/packages)
[![registry status badge](https://rotsl.r-universe.dev/badges/\:registry)](https://rotsl.r-universe.dev/)
[![articles status badge](https://rotsl.r-universe.dev/badges/\:articles)](https://rotsl.r-universe.dev/articles)

---

## Cave Packages

### 1. grayleafspotr

Tool for look at gray leaf spot things in RStudio.

[![R-universe](https://img.shields.io/badge/R--universe-grayleafspotr-blue)](https://rotsl.r-universe.dev/grayleafspotr)
[![GitHub](https://img.shields.io/badge/GitHub-rotsl%2Fgrayleafspotr-black)](https://github.com/rotsl/grayleafspotr)

Quantitative phenotyping tools for gray leaf spot fungal colonies grown on petri dishes.

Use it to:

* Find gray leaf spot colonies
* Measure colony things
* Make plots
* Make tidy results
* Work with time-series plate images

---

### 2. grayleafspotdata

Data map for gray leaf spot image things.

[![R-universe](https://img.shields.io/badge/R--universe-grayleafspotdata-blue)](https://rotsl.r-universe.dev/grayleafspotdata)
[![GitHub](https://img.shields.io/badge/GitHub-rotsl%2Fgrayleafspotdata-black)](https://github.com/rotsl/grayleafspotdata)

Provides machine-readable file and image manifests for the **S-BSST3199 Magnaporthe colony image dataset**.

Big research files stay in their original data cave. Package gives tidy maps so R can find what lives where without stuffing all pictures inside the package.

Data things include:

* `grayleafspot_files` — deposited file manifest
* `grayleafspot_images` — individual colony image manifest

Good for:

* Finding gray leaf spot research files
* Finding individual colony images
* Reproducible image-analysis workflows
* Plant-pathology workflows
* Feeding image information into `grayleafspotr`

See package:

https://rotsl.r-universe.dev/grayleafspotdata

See all data things:

https://rotsl.r-universe.dev/datasets

---

## Installation

Put both packages in R like this:

```r
install.packages(
  c("grayleafspotr", "grayleafspotdata"),
  repos = c(
    "https://rotsl.r-universe.dev",
    "https://cloud.r-project.org"
  )
)
```

Or put package in one at a time:

```r
install.packages(
  "grayleafspotr",
  repos = c(
    "https://rotsl.r-universe.dev",
    "https://cloud.r-project.org"
  )
)

install.packages(
  "grayleafspotdata",
  repos = c(
    "https://rotsl.r-universe.dev",
    "https://cloud.r-project.org"
  )
)
```

---

## Data Cave

Load data maps:

```r
library(grayleafspotdata)

data("grayleafspot_files")
data("grayleafspot_images")

head(grayleafspot_files)
head(grayleafspot_images)
```

Or poke things directly:

```r
grayleafspotdata::grayleafspot_files
grayleafspotdata::grayleafspot_images
```

Browse all rotsl datasets:

[![R-universe datasets](https://img.shields.io/badge/R--universe-datasets-blue)](https://rotsl.r-universe.dev/datasets)

---

## Big Scrolls

[Read grayleafspotr package wisdom here](https://rotsl.github.io/grayleafspotr/)

Find:

* What functions do
* Story scrolls and examples
* How put package in R
* How use package
* New updates?

More package caves:

* [grayleafspotr on R-universe](https://rotsl.r-universe.dev/grayleafspotr)
* [grayleafspotdata on R-universe](https://rotsl.r-universe.dev/grayleafspotdata)
* [rotsl datasets](https://rotsl.r-universe.dev/datasets)

---

## Magic Demo Cave

Try leaf spot machine here:

* [Demo cave](https://huggingface.co/spaces/rotsl/grayleafspot-segmentation-demo)
* [Model cave](https://huggingface.co/rotsl/grayleafspot-segmentation-demo)

[![License](https://img.shields.io/badge/License-Apache%202.0-green.svg)](https://opensource.org/licenses/Apache-2.0)
[![DOI](https://img.shields.io/badge/DOI-10.57967%2Fhf%2F8569-orange)](https://doi.org/10.57967/hf/8569)

Magic cave do:

* Put pictures in
* Find gray leaf spot
* Make overlay picture
* Make plots
* Give CSV and JSON files
* Pack all things in ZIP bundle

---

## Cave Family

```text
grayleafspotdata
      |
      |  tells where data things live
      v
image + file manifests
      |
      |  feed image things into analysis
      v
grayleafspotr
      |
      |  segment + measure + plot
      v
results, pictures, plots, CSV, JSON
```

Data cave gives map.

Analysis cave does science things.

Happy.
