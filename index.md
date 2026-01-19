---
layout: default
title: Portfolio
---

## Bio
I am a Doctoral Researcher at Pennsylvania State University. I build physics-grounded, data-driven methods to extract actionable information from radar sensing data. This portfolio highlights selected publications and additional projects, including works in progress and smaller explorations that are not standalone papers but demonstrate my approach, tooling, and technical range.

---

## Publications

### Data-driven evaluation of building materials using Ground Penetrating Radar
A data-driven approach for predicting material type and layer thickness from GPR scans is proposed. The methodology also successfully detects sub-wavelength thicknesses. [Read more](https://www.sciencedirect.com/science/article/pii/S235271022401756X).

<figure style="text-align:center; margin: 1.2rem 0;">
  <img src="{{ 'gifs/bottom_layer_reflection.gif' | relative_url }}" alt="Figure 1: Subwavelength interfaces produce discernible signal patterns." style="max-width: 380px; width: 100%; height: auto;">
  <figcaption><strong>Figure 1:</strong> Supposedly indiscernible reflections from interfaces with subwavelength separation are accurately predicted using data-driven methods.</figcaption>
</figure>

<figure style="text-align:center; margin: 1.2rem 0;">
  <img src="{{ 'assets/img/workflow_diagram.png' | relative_url }}" alt="Figure 2: Workflow diagram for predicting material type and subwavelength thickness." style="max-width: 900px; width: 100%; height: auto;">
  <figcaption><strong>Figure 2:</strong> Both material type and subwavelength sample thickness values were correctly predicted by the proposed model.</figcaption>
</figure>

### Interpretable AI for Building Envelope Inversion (submitted)
Building envelopes represent a challenge for GPR due to their lower permittivity contrasts and comparatively cluttered interiors. This work proposes a data-driven framework utilizing sparse neural networks for diagnosing building envelopes using GPR signals. The framework is accurate, interpretable, and robust to spurious patterns.

<figure style="text-align:center; margin: 1.2rem 0;">
  <img src="{{ 'paper-2-overview.PNG' | relative_url }}" alt="Figure 3: Overview of building envelope reflections and sparse neural network interpretation." style="max-width: 1000px; width: 100%; height: auto;">
  <figcaption><strong>Figure 3:</strong> (left) Complex reflections within building envelope interior, (center) Sparse neural network interprets signals while trimming low-quality features, (right) Selected features map to salient locations in the building envelope.</figcaption>
</figure>

---

## Conferences
- **ASCE Engineering Mechanics Institute 2022 Conference** — Brief description of the presentation. [Abstract (see page 8)](https://www.emi-conference.org/sites/emi-conference.org/2022/files/inline-files/EMI%202022%20Book%20of%20Abstracts.pdf).
- **ASCE Engineering Mechanics Institute 2023 Conference** — Brief description of the presentation. [Abstract (see page 30)](https://www.asce.org/-/media/798f777f1bb446ceb8a290267b11cb79.ashx).
- **ASCE Engineering Mechanics Institute 2024 Conference** — Brief description of the presentation. [Abstract (see page 8)](https://www.asce.org/-/media/798f777f1bb446ceb8a290267b11cb79.ashx).

---

## Works in Progress

### GPR Scan Inversion Using Deep Neural Network
A generative model inverts GPR B-scans for a buried object problem. A relatively light VAE model accurately indicates the object position and size, although results are inconclusive when the buried object is small. [See project details]({{ 'DNN-inversion/README.md' | relative_url }}).

<figure style="text-align:center; margin: 1.2rem 0;">
  <img src="{{ 'DNN-inversion/img/DNN_inversion_AE.PNG' | relative_url }}" alt="Figure 4: VAE models the joint distribution between permittivity maps and B-scans." style="max-width: 720px; width: 100%; height: auto;">
  <figcaption><strong>Figure 4:</strong> A Variational Autoencoder (VAE) models the joint distribution between permittivity-map geometries and their corresponding B-scans, enabling computationally efficient inversion.</figcaption>
</figure>

### Orientation Detection for Angular Defects in Building Envelopes
This study investigates convolutional neural networks (CNNs) for detecting building envelope defects. A controlled experiment rotates an isosceles triangular defect within a building envelope; GPR B-scans are simulated using an FDTD solver (gprMax). A convolutional regression model predicts defect orientation from radargrams. [See project details](https://nirjharalam.github.io/triangular_defect/).

<figure style="text-align:center; margin: 1.2rem 0;">
  <img src="{{ 'gifs/triangular_defect_orientation_data1-ezgif.com-loop-count.gif' | relative_url }}" alt="Figure 5: Orientation sweep example for a triangular defect." style="max-width: 820px; width: 100%; height: auto;">
  <figcaption><strong>Figure 5:</strong> Although a continuous shift is observed with a change in orientation, this pattern breaks down when the sharp corners of the defect are oriented toward the incoming GPR signals.</figcaption>
</figure>
