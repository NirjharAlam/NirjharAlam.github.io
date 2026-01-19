# Ahmed Nirjhar Alam's Portfolio

<div align="left">
    <img src="./assets/img/rough_snip.png" alt=Both material type and subwavelength sample thickness values were correctly predicted by the proposed model." width="200">
</div>

## Bio


I am a Doctoral Researcher at Pennsylvania State University. I build physics-grounded, data-driven methods to extract actionable information from radar sensing data. This portfolio highlights selected publications and additional projects, including works in progress and smaller explorations that are not standalone papers but demonstrate my approach, tooling, and technical range.


## Publications
- **Data-driven evaluation of building materials using Ground Penetrating Radar**  
  A data-driven approach for predicting material type and layer thickness from GPR scans is proposed. The methodology also successfully detects sub-wavelength thicknesses. [Read more](https://www.sciencedirect.com/science/article/pii/S235271022401756X).



<div align="center">
    <img src="./gifs/bottom_layer_reflection.gif" Simulation revealed subwavelength layers produced discernible signal patterns for both interfaces" width="300">
    <p><strong>Figure 1:</strong> Supposedly indiscernible reflections from interfaces with subwavelength separation are accurately predicted using data-driven methods.</p>
</div>



<div align="center">
    <img src="./assets/img/workflow_diagram.png" alt=Both material type and subwavelength sample thickness values were correctly predicted by the proposed model." width="800">
    <p><strong>Figure 2:</strong> Both material type and subwavelength sample thickness values were correctly predicted by the proposed model.</p>
</div>



- **Interpretable AI for Building Envelope Inversion (*submitted*)**  
  Building envelopes represent a challenge for GPR, due to their lower permittivity contrasts and comparatively cluttered interiors. This work proposes a data-driven framework, utilizing sparse neural networks, for diagnosing building envelopes using GPR signals. The proposed framework is accurate, highly interpretable, and robust to spurious patterns in the signal.




<div align="center">
    <img src="./paper-2-overview.PNG" alt=Simulation revealed subwavelength layers produced discernible signal patterns for both interfaces" width="12000">
    <p><strong>Figure 3:</strong> (left) Complex reflections within building envelope interior, (center) Sparse neural network interprets signals while trimming low-quality features, (right) Selected features  map to salient locations
        in the building envelope.</p>
</div>





## Conferences
- **ASCE Engineering Mechanics Institute 2022 Conference**  
  Brief description of the presentation. [Abstract (see page 8)](https://www.emi-conference.org/sites/emi-conference.org/2022/files/inline-files/EMI%202022%20Book%20of%20Abstracts.pdf).

- **ASCE Engineering Mechanics Institute 2023 Conference**  
  Brief description of the presentation. [Abstract (see page 30)](https://www.asce.org/-/media/798f777f1bb446ceb8a290267b11cb79.ashx).

- **ASCE Engineering Mechanics Institute 2024 Conference**  
  Brief description of the presentation. [Abstract (see page 8)](https://www.asce.org/-/media/798f777f1bb446ceb8a290267b11cb79.ashx)


## Works in Progress
- **GPR Scan Inversion Using Deep Neural Network**  
  A generative model inverts GPR B-scans for a buried object problem. A relatively light VAE model accurately indicates the objects' position and size, although results are inconclusive when the buried object is small. [See project details](./DNN-inversion/README.md).
  
  <div align="center">
    <img src="./DNN-inversion/img/DNN_inversion_AE.PNG" alt=Simulation revealed subwavelength layers produced discernible signal patterns for both interfaces" width="500">
    <p><strong>Figure 4:</strong> A Variational Autoencoder (VAE) models the joint distribution between input geometries - represented as permittivity maps of subsurface structures - and their corresponding B-scans. This enables computationally efficient full-waveform inversion of GPR data for target configurations. </p>
</div>


- **Orientation Detection for Angular Defects in Building Envelopes**
This study investigates the potential of convolutional neural networks (CNNs) for detecting building envelope defects. A controlled experiment is designed in which an isosceles triangular defect is rotated within a building envelope. At each point, the corresponding GPR B-scan of the wall section is simulated using an FDTD solver (GPRMax). A convolutional regression model is trained to predict defect orientation from the radargrams. [See project details](https://nirjharalam.github.io/triangular_defect/).

  <div align="center">
    <img src="./gifs/triangular_defect_orientation_data1-ezgif.com-loop-count.gif" alt=Simulation revealed subwavelength layers produced discernible signal patterns for both interfaces" width="600">
    <p><strong>Figure 5:</strong> Although a continuous shift is observed with a change in orientation, this pattern breaks down when the sharp corners of the defect are oriented toward the incoming GPR signals. </p>
</div>


