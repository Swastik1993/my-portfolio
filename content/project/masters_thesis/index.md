---
title: Entropy based Fuzzy clustering algorithm for MR image segmentation
summary: Used Shannon entropy to modify the Fuzzy C-Means algorithm for segmenting volumetric brain MR images, model was evaluated on the Brainweb dataset and IBSR dataset before utilizing for the real-patient image volumes

tags:
- BioInformatics
- Brain MRI
- Image segmentation
- Clustering algorithms
- Shannon Entropy
- Gaussian density function
- Fuzzy C-Means clustering
date: "2019-03-30T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: Segmented Brain MR Image
  focal_point: Smart

# links:
# - icon: twitter
#   icon_pack: fab
#   name: Follow
#   url: https://twitter.com/georgecushen
url_code: ""
url_pdf: "/publication/icinpro/icinpro.pdf"
url_slides: ""
url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ""
---

Brain MR image segmentation has gained popularity in recent past due to its nature of treatment and consistent search for near perfect clinical diagnosis and analysis. There are numerous different types of methods for MR image segmentation have been proposed. However, among them, the fuzzy logic based clustering algorithms are studied more as it deals with uncertainties that arise while classifying pixels into possible brain soft tissue regions. 

But, conventional fuzzy clustering algorithm like fuzzy c-means (FCM) algorithm does not consider spatial information, thereby limiting its performance, especially when the brain MR images are corrupted by high noise and intensity inhomogeneity (IIH). As brain MR images are contaminated by noise and intensity inhomogeneity (IIH), achieving accurate segmentation results quite difficult and challenging task

We have proposed a fuzzy entropy based clustering algorithm for segmentation of volumetric noisy brain MR image data. For each voxel under consideration, we have defined likeliness measures corresponding to all clusters from its cubic local neighborhood region. These measures are finally used to introduce fuzzy entropy that defines the vagueness and information uncertainty while identifying the possible cluster or class. Therefore, better representation and utilization of this information uncertainty into a fuzzy clustering algorithm will lead to a possible solution of the problem. 

To realize this we have utilized intensity distribution in a spatial cubic local neighborhood to measure a possibility factor that defines likeliness of the voxel under consideration to belong into a cluster or region. To mitigate the affects of noise and IIH we judiciously define a Gaussian density function. Afterwards these likeliness measures are normalized so as to consider them as an alternative membership function. The fuzzy membership function and this normalized likeliness measure are incorporated into the objective function using a regularizing parameter. Additionally, normalized likeliness measure based fuzzy entropy defined by Shannon’s function is introduced to represent the vagueness and ambiguity uncertainty while classifying a voxel into its possible cluster. Therefore, this framework makes the cluster prototypes to utilize the fuzzy membership functions, likeliness measures and fuzzy entropy.

This proposed algorithm is extensively studied both in qualitatively and quantitatively on simulated and clinical brain MR image volumes with high noise and IIH. The performance of it is superior to some of the state-ofthe-art algorithms.
