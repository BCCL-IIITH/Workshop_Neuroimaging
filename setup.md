# Before the workshop

> # Hands-on 
> - Software Carpentry <a href="https://swcarpentry.github.io/shell-novice">Unix</a> and/or <a href="https://swcarpentry.github.io/python-novice-inflammation">Python</a>
> - Tal Yarkoni's <a href="https://neurohackademy.org/course/introduction-to-python-2/">"Introduction to Python" lecture delivered at Neurohackademy 2019</a>
> - Gaël Varoquaux's <a href="https://gael-varoquaux.info/scipy-lecture-notes/">Scipy Lecture Notes</a> 
> - J. R. Johansson <a href="http://github.com/jrjohansson/scientific-python-lectures">IPython notebooks</a> 

# Installations

## Python 3 via Miniconda (recommended)
    conda create -n nimg_workshop python=3.9
    conda activate nimg_workshop

## Install Python packages
Pip is the most common package installer for Python. This session requires a few additional neuroimaging-specific Python packages that can be installed with:

    pip install nibabel nilearn pybids

<a href="nilearn.github.io">`nilearn`</a> and <a href="https://nipy.org/nibabel/">`nibabel`</a> are for Neuroimaging data loading & handling; <a href="https://bids-standard.github.io/pybids/">`pybids`</a> for organizing neuroimaging data in proper structure

    pip install pandas

<a href="https://pandas.pydata.org/(https://pandas.pydata.org/)">`pandas`</a> is for non-imaging data loading

## Install dcm2niix

<a href="https://github.com/rordenlab/dcm2niix#install"> `dcm2niix`</a> software package for converting neuroimaging data from the DICOM format that is exported from the MRI scanner to the NIfTI format. Detailed installation instructions for various operating systems can be found on the `dcm2niix` <a href="https://github.com/rordenlab/dcm2niix#install"> README</a>. With the Anaconda Python distribution which is recommended, `dcm2niix` can be installed by:

    conda install -c conda-forge dcm2niix

## Test launching Python Interface

Jupyter notebook
IPython Interpreter
Google Colab
