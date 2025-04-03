# Guide to Jupyterhub Kernels on I-GUIDE

On I-GUIDE, we have various kernels available in Jupyterhub. These originate from I-GUIDE and CyberGISX. This document explains what each kernel contains and why you'd want to use each one.

### iguide kernel

The basic iguide kernel has most packages you would want to use (GDAL, geopandas, rasterio, etc), and you should default to it if you don't know what to pick.

### iguide-ewd kernel

This is similar to the iguide kernel, but features specific packages for the EWD team on I-GUIDE. It features tensorflow, for example.

### geoai kernel

This kernel is meant for AI / machine learning. It has PyTorch, Natural Language Toolkit, spaCy, and HuggingFace Transformers. Don't confuse this with geoai-Python3, which is a CyberGISX kernel and should be use for Notebooks coming from CyberGISX.

### iguide-ewd-r kernel

This is our R kernel. It's the main kernel for any R programming.

### CyberGISX kernels

We have other kernels available on the platform. These are from CyberGISX. These are here if you are porting a Notebook from CyberGISX.

### How to view all packages in a kernel

Type this command in Jupyterhub's terminal to view a specific kernel on I-GUIDE

`conda env export --p /cvmfs/iguide.purdue.edu/software/conda/<kernel_name>`


You can view a list of kernels by typing

`ls /cvmfs/iguide.purdue.software/conda/`

