# MeMo NF (Merge Model between Neural Field)

## Preliminaries
### Neural Radiance Field (NeRF)
The Neural Radiance Fields (NeRF) model is a method for synthesizing novel views of complex scenes by directly optimizing a continuous volumetric scene representation. Unlike traditional 3D representation methods, NeRF uses a fully connected (non-convolutional) network, trained to map 5D coordinates to colors. The 5D coordinates contain both spatial location (3D) and viewing direction (2D). This method achieves state-of-the-art results on view synthesis benchmarks and can render high-quality novel views that are consistent with the observed data.

<p align="center">
 <img src = "./image/nerf.png">
</p>

### Tiny NeRF
The difference between Tiny NeRF and NeRF is input shape and deepness of the model. In our case, we used 3D coordinates for model inputs dimesion reducted with encoding function. 
We reduced not only input shape, but also model architectures because of complexity. 

<p align="center">
 <img src = "./image/tinynerf_architecture.png">
</p>

### Model Merging Method
There are so many Model merging Method.
 1. random mix model merging
 2. Fisher weighted mix parameter
 3. REPAIR

We applied all of the Model Merging Methods.

