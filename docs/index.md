# Designing for Discovery: Shaping Imageomics Tools for Biologists

A hands-on workshop at [Evolution 2026](https://www.evolutionmeeting.org/) in Cleveland, OH, hosted by the [Imageomics Institute](https://imageomics.osu.edu/).

- **Date:** Saturday, June 20, 2026, 1:00-5:00 PM
- **Location:** Cleveland, OH (Evolution 2026)
- **Program:** [Official Evolution 2026 program listing](https://www.xcdsystem.com/evolution/program/o5SCPR5/index.cfm)

---

## About

Imageomics is an emerging interdisciplinary field at the crossroads of machine learning (ML), computer vision (CV), and biological sciences. It leverages visual data, from microscopic images of unicellular organisms to videos of megafauna, to extract and analyze biological traits. By grounding ML models in existing scientific knowledge, the emerging field of imageomics aims to make traits computable from images and videos, facilitating insights into the evolution and function of living organisms. 

This half-day workshop focuses on making imageomics tools more accessible and usable for biologists and will be centered on co-development, where tool refinement and new use cases emerge through active partnership with biologists. During the workshop, selected Imageomics Institute tools for taxonomic identification and trait segmentation, exploration, and classification will be demonstrated. 

We will highlight the potential applications of these tools toward facilitating the measurement of evolutionary traits for biodiversity science, systematics, and evolutionary biology, as well as the measurement of complex traits such as behaviors from videos. 

## Schedule

| Time | Session | Led by |
|------|---------|--------|
| 1:00 - 1:15 | **Introduction & Overview of Imageomics** | Wei-Lun (Harry) Chao, PhD |
| 1:15 - 1:45 | **Tools & ML Background**: an overview of the tools and the machine learning ideas behind them, with use cases across birds, beetles, and butterflies | Caleb Charpentier & Jianyang Gu, PhD |
| 1:45 - 5:00 | **Hands-on Tutorials** (with breaks and open discussion) | Assorted |

## Tutorials

Each tutorial walks through a specific Imageomics tool, from setup to hands-on use with example data. Most run end-to-end in Google Colab. Open the notebook, make a copy, and run the cells as we go.

### pybioclip

_Led by Matthew Thompson, PhD_

> Classify focal species and generate image embeddings programmatically using BioCLIP family models, without complex ML infrastructure.

`pybioclip` is a Python package that puts the [BioCLIP family of foundation models](https://imageomics.github.io/bioclip-ecosystem/pages/models.html) a few lines of code away. Use it to predict taxonomic labels for an image, score images against your own list of candidate species, and extract embeddings for downstream analysis.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Imageomics/evolution-workshop-2026/blob/main/docs/tutorials/notebooks/pybioclip.ipynb)

### Image Embedding Explorer

_Led by Net Zhang_

> Explore sets of image embeddings interactively. Try different models and projections. See which images cluster together or separate.

The Image Embedding Explorer turns a folder of images into an interactive map. Compare embedding models, switch between projection methods, and visually inspect how organisms group by trait and taxonomy. This offers quick way to build intuition for how a model "thinks" about relationships among images and to explore the structure of your data.

[![Open in Spaces](https://huggingface.co/datasets/huggingface/badges/resolve/main/open-in-hf-spaces-md.svg)](https://huggingface.co/spaces/netzhang/emb-explorer-demo)

### BioCLIP Image Search Lite

_Led by Net Zhang_

> Given a query image of an organism, find the most visually similar images across 200M+ samples from the TreeOfLife dataset.

BioCLIP Image Search Lite is a lightweight similarity search over the [TreeOfLife](https://huggingface.co/datasets/imageomics/TreeOfLife-200M) collection. Upload a query image and retrieve the closest matches by BioCLIP embedding. This is a fast way to find related organisms and surface visually similar specimens at scale.

[![Open in Spaces](https://huggingface.co/datasets/huggingface/badges/resolve/main/open-in-hf-spaces-md.svg)](https://huggingface.co/spaces/imageomics/bioclip-image-search-lite)

### SST (Static Segmentation by Tracking)

_Led by Fangxun Liu_

> Segment traits from specimen images with just a handful of labeled examples.

Static Segmentation by Tracking (SST) treats a set of specimen images like frames in a video: label the traits on one (or a few) examples, and SST propagates those segmentations to the rest of your collection. This tutorial covers running SST in one-shot and few-shot settings, and extending it to search for images with similar traits.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1Iv3U-ftspiNmbSKbsneoA1Ipk7NpLvm5?usp=sharing)

## Acknowledgments

Many people shaped this workshop. Our thanks to everyone who contributed ideas, feedback, and planning, alongside the instructors listed above, including Diane Boghrat, Niko Zuppas, Josef Uyeda, Hilmar Lapp, Elizabeth Campolongo, Jake Beattie, Sydne Record, Eric Sokol, and Tanya Berger-Wolf.



The Imageomics Institute is supported by the National Science Foundation under Award No. 2118240. Any opinions, findings and conclusions or recommendations expressed in this material are those of the author(s) and do not necessarily reflect the views of the National Science Foundation.
