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

### Journals Papers:
1. Ahmed, M., & Qin, N. (2009). *Surrogate-Based Aerodynamic Design Optimization: Use of Surrogates in Aerodynamic Design Optimization*. Aerospace Sciences and Aviation Technology, ASAT-13.
2. Balabanov, V., Giunta, A., Golovidov, O., Grossman, B., Mason, H., Watson, T., & Haftkalf, T. (1999). *Reasonable Design Space Approach to Response Surface Approximation*. Journal of Aircraft.
3. Batill, M., Stelmack, A., & Sellar, S. (1999). *Framework for Multi-disciplinary Design Based on Response-Surface Approximations*. Journal of Aircraft.
4. Bengio, Y. (2009). *Learning Deep Architectures for AI*. Foundations and Trends in Machine Learning.
5. Chittka, L., Skorupski, P., & Raine, E. (2009). *Speed-Accuracy Tradeoffs in Animal Decision Making*. Trends in Ecology and Evolution.
6. Eigen, D., Puhrsch, C., & Fergus, R. (2014). *Depth Map Prediction from a Single Image Using a Multi-Scale Deep Network*. Advances in Neural Information Processing Systems.
7. Fang, H., Rais-Rohani, M., Liu, Z., & Horstemeyer, M. (2005). *A Comparative Study of Metamodeling Methods for Multi-Objective Crashworthiness Optimization*. Computers & Structures.
8. Giunta, A. (1997). *Aircraft Multidisciplinary Design Optimization Using Design of Experiments Theory and Response Surface Modeling Methods*.
9. Gupta, S., Girshick, R., Arbelaez, P., & Malik, J. (2014). *Learning Rich Features from RGB-D Images for Object Detection and Segmentation*. In Computer Vision, ECCV.
10. Hartmann, D., Meinke, M., & Schroder, W. (2008). *Differential Equation Based Constrained Reinitialization for Level Set Methods*. Journal of Computational Physics.
11. Heuveline, V., & Latt, J. (2007). *The OpenLB Project: An Open Source and Object-Oriented Implementation of Lattice Boltzmann Methods*. International Journal of Modern Physics.
12. Jeong, S., Murayama, M., & Yamamoto, K. (2005). *Efficient Optimization Design Method Using Kriging Model*. Journal of Aircraft.
13. Leary, S. J., Bhaskar, A., & Keane, A. J. (2004). *Global Approximation and Optimization Using Adjoint Computational Fluid Dynamics Codes*. AIAA Journal.
14. Tran, D., Bourdev, L., Fergus, R., Torresani, L., & Paluri, M. (2015). *Deep End2end Voxel2voxel Prediction*. arXiv preprint arXiv:1511.06681.
15. Wilkinson, S., Bradbury, G., & H. S. (2015). *Reduced-Order Urban Wind Interference*. Simulation: Transactions of the Society for Modeling and Simulation International.
16. Russo, G., & Smereka, P. (2000). *A Remark on Computing Distance Functions*. Journal of Computational Physics.
17. Mawson, M., Leaver, G., & Revell, A. (2013). *Real-Time Flow Computations Using an Image-Based Depth Sensor and GPU Acceleration*.
18. McNamara, G. R., & Zanetti, G. (1988). *Use of the Boltzmann Equation to Simulate Lattice-Gas Automata*. Physical Review Letters.
19. Patankar, S. (1980). *Numerical Heat Transfer and Fluid Flow*. CRC Press.
20. Socher, R., Huval, B., Bath, B., Manning, C. D., & Ng, A. Y. (2012). *Convolutional-Recursive Deep Learning for 3D Object Classification*. Advances in Neural Information Processing Systems.

### Books:
1. Anderson, J. (1995). *Computational Fluid Dynamics*.
2. Forsythe, G., & Wasow, W. (1960). *Finite-Difference Methods for Partial Differential Equations*.
3. Schmidhuber, J. (2015). *Deep Learning in Neural Networks: An Overview*. Neural Networks.

### Conference Proceedings:
1. Daberkow, D., & N. D. (1998). *New Approaches to Conceptual and Preliminary Aircraft Design: A Comparative Assessment of a Neural Network Formulation and a Response Surface Methodology*. World Aviation Conference.
2. Dosovitskiy, A., Fischer, P., Ilg, E., Hausser, P., Hazrba, C., Golkov, V., Smagt, P. v. d., Cremers, D., & Brox, T. (2015). *Flownet: Learning Optical Flow with Convolutional Networks*. In IEEE International Conference on Computer Vision (ICCV).
3. Jia, Y., Shelhamer, E., Donahue, J., Karayev, S., Long, J., Girshick, R., & Darrell, T. (2014). *Convolutional Architecture for Fast Feature Embedding*. In Proceedings of the ACM International Conference on Multimedia.
4. LeCun, Y., Bottou, L., Bengio, Y., & Haner, P. (1998). *Gradient-Based Learning Applied to Document Recognition*. Proceedings of the IEEE.
