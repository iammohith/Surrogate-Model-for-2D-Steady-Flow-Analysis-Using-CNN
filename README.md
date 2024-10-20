# Surrogate Model for 2D Steady Flow Analysis Using CNN

## Abstract
In aerodynamics-related design, analysis, and optimization problems, flow fields are simulated using computational fluid dynamics (CFD) solvers. However, CFD simulations are computationally expensive, memory-intensive, and time-consuming, limiting design space exploration and prohibiting interactive design.

We propose a general and flexible approximation model for real-time prediction of uniform steady laminar flow in a 2D domain based on convolutional neural networks (CNNs). This approach explores alternatives for geometry representation and CNN architecture. Our CNN model estimates the velocity field two orders of magnitude faster than a GPU-accelerated CFD solver and four orders faster than a CPU-based CFD solver, while maintaining a low error rate.

This model provides immediate feedback for real-time design iterations at the early stages. Unlike existing approximation models in aerodynamics, CNNs enable efficient estimation of the entire velocity field. Designers and engineers can apply the CNN approximation model directly in their design space exploration algorithms without training additional lower-dimensional surrogate models.

## Contents
1. **Certificate**
2. **Declaration**
3. **Abstract**
4. **Acknowledgement**
5. **List of Figures**
6. **List of Tables**
7. **Chapter 1: Introduction**
   - Computational Fluid Dynamics
   - Finite Volume Method
   - Surrogate Modeling in CFD
   - Convolutional Neural Networks (CNN)
   - Architecture, Features, Hyperparameters, and Applications
   - Image Segmentation
8. **Chapter 2: Literature Review**
   - Literature Survey
   - Motivation for Present Work
9. **Chapter 3: Objectives and Methodology**
   - Geometry Representation
   - UNet Model Architecture
10. **Chapter 4: Numerical Analysis**
    - CFD Simulation
    - CNN and UNet Model Analysis
11. **Chapter 5: Results and Discussions**
    - CNN Results
    - Predicted Images and Computational Time
12. **Chapter 6: Conclusions**
13. **References**

## Conclusion
We successfully built a surrogate model for 2D steady-state laminar flow. However, due to the limited dataset, predictions were moderate. Future work will focus on increasing the dataset size and improving prediction quality.

Despite preparing a colored image dataset, technical limitations forced us to switch to grayscale images. Future efforts will restore the use of colored images for improved accuracy.

Our primary goal is to offer a lightweight (fast but less accurate) surrogate model for exterior flow. While low Reynolds number flows suffice for certain domains like architectural design, we aim to extend this approach to higher Reynolds number flows in the future. Additionally, the CNN approximation model could be used to accelerate traditional CFD simulations by providing a more efficient initial setup, significantly reducing the time to convergence.

## References
**Journals**:
1. M. Ahmed and N. Qin. *Surrogate-Based Aerodynamic Design Optimization*, Aerospace Sciences and Aviation Technology, ASAT-13, 2009.
2. V. Balabanov et al. *Reasonable Design Space Approach to Response Surface Approximation*, Journal of Aircraft, 1999.
3. M. Batill et al. *Framework for Multi-Disciplinary Design Based on Response Surface Approximations*, Journal of Aircraft, 1999.
4. Y. Bengio. *Learning Deep Architectures for AI*, Foundations and Trends in Machine Learning, 2009.
