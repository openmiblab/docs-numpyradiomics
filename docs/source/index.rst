.. dbdicom documentation master file, created by
   sphinx-quickstart on Mon Oct 10 07:46:23 2022.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

##############
NumpyRadiomics
##############

A lightweight, pure-Python implementation of radiomic shape and 
texture features, fully compatible with **PyRadiomics** definitions. 
Built on top 
of `numpy`, `scipy`, and `skimage` to minimize heavy dependencies 
while maintaining accuracy.

Features
########

- **Standard Compliance**: Implements the official PyRadiomics definitions for texture and shape features.
- **Lightweight**: No heavy C++ extensions or SimpleITK dependencies required—just standard scientific Python stacks.


Installation
############

.. code-block:: bash

   pip install numpyradiomics


Supported Features
##################

3D Shape (Standard)
-------------------

- **Volume**: Mesh Volume, Voxel Volume
- **Surface**: Surface Area, Surface-to-Volume Ratio
- **Dimensions**: Max 3D Diameter, Max 2D Diameter (Slice, Column, Row)
- **Shape Descriptors**: Sphericity, Elongation, Flatness
- **Axes**: Major, Minor, and Least Axis Lengths

3D Shape (Extended)
-------------------

- **Advanced Volume**: Convex Hull Volume, Bounding Box Volume
- **Ratios**: Solidity, Extent
- **Inertia**: Moments of Inertia, Fractional Anisotropy
- **Other**: Maximum Depth (Chebyshev Radius), Longest Caliper Diameter

2D Shape
--------

- **Area**: Mesh Surface, Pixel Surface
- **Perimeter**: Perimeter, Perimeter-Surface Ratio
- **Shape Descriptors**: Sphericity, Spherical Disproportion, Elongation
- **Axes**: Major Axis, Minor Axis, Max Diameter

Texture
-------

All standard texture metrics are available:

- **GLCM**: Gray Level Co-occurrence Matrix
- **GLRLM**: Gray Level Run Length Matrix
- **GLSZM**: Gray Level Size Zone Matrix
- **GLDM**: Gray Level Dependence Matrix
- **NGTDM**: Neighbouring Gray Tone Difference Matrix

License
-------

Apache 2.0 License


.. toctree::
   :maxdepth: 2
   :hidden:
   
   user_guide/index
   reference/index
   about/index