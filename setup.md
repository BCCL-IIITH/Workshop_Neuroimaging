# Before the workshop: Installations and Data downloading

> # Hands-on 
> - Software Carpentry <a href="https://swcarpentry.github.io/shell-novice">Unix</a> and/or <a href="https://swcarpentry.github.io/python-novice-inflammation">Python</a>
> - Tal Yarkoni's <a href="https://neurohackademy.org/course/introduction-to-python-2/">"Introduction to Python" lecture delivered at Neurohackademy 2019</a>
> - Gaël Varoquaux's <a href="https://gael-varoquaux.info/scipy-lecture-notes/">Scipy Lecture Notes</a> 
> - J. R. Johansson <a href="http://github.com/jrjohansson/scientific-python-lectures">IPython notebooks</a> 

# Installation options at your will

## Python 3 via Miniconda
After conda installation, one can create a separate conda environment specific to this workshop, without necessarily disturbing your own research specific installation packaging versions.

    conda create -n nimg_workshop python=3.9
    conda activate nimg_workshop

## Install Python packages
Pip is the most common package installer for Python. This session requires a few additional neuroimaging-specific Python packages that can be installed with:

    pip install nibabel nilearn pybids

<a href="nilearn.github.io">`nilearn`</a> and <a href="https://nipy.org/nibabel/">`nibabel`</a> are for Neuroimaging data loading & handling; <a href="https://bids-standard.github.io/pybids/">`pybids`</a> for organizing neuroimaging data in proper structure

    pip install pandas

<a href="https://pandas.pydata.org/(https://pandas.pydata.org/)">`pandas`</a> is for non-imaging data loading

    pip install matplotlib

<a href="https://matplotlib.org/(https://matplotlib.org/)">`matplotlib`</a> is for visualization

## Install dcm2niix

<a href="https://github.com/rordenlab/dcm2niix#install"> `dcm2niix`</a> software package for converting neuroimaging data from the DICOM format that is exported from the MRI scanner to the NIfTI format. Detailed installation instructions for various operating systems can be found on the `dcm2niix` <a href="https://github.com/rordenlab/dcm2niix#install"> README</a>. With the Anaconda Python distribution which is recommended, `dcm2niix` can be installed by:

## Install MRIcron GUI interface for DICOM to Nifti converter

### Alternative to command line execution

<a href="https://people.cas.sc.edu/rorden/mricron/install.html"> `MRIcron installation`</a>

## Install Python Interface

[Jupyter notebook](https://jupyter.org/)

[IPython Interpreter](https://ipython.org/install.html)

[Google Colab](https://colab.research.google.com/) No installation as such, just use with Google login

## Install FSL for brain templates and fMRI processing

<a href="https://fsl.fmrib.ox.ac.uk/fsl"> `FSL - FMRIB Software Library`</a>

## Install freesurfer for T1-weighted MR processing

<a href="https://surfer.nmr.mgh.harvard.edu/"> `Freesurfer Software Suite`</a>

## [Installing Python Packages from a Jupyter Notebook](https://jakevdp.github.io/blog/2017/12/05/installing-python-packages-from-jupyter/)


# After installation, please check the installation

For e.g., Try importing nilearn in a python / iPython session:

```python
import nilearn
```
If no error is raised, you have installed nilearn correctly.

Similary, check for `nibabel` `pandas`, etc.


# Download sample DICOM data

You can download the sample data either using internet browser or via command line.

From an internet browser simply navigate to this [link](https://zenodo.org/record/3677090) and click Download option there.

Command line download option for Linux/MaxOS

    wget https://zenodo.org/record/3677090/files/0219191_mystudy-0219-1114.tar.gz

## After the download

Navigate to the directory where data is downloaded, then you can unzip and extract files from the tarball (tar archive) using the following command:

    tar -xvzf 0219191_mystudy-0219-1114.tar.gz
    gzip -d 0219191_mystudy-0219-1114/dcm/*dcm.gz

Data source: A Big Thanks to [The Princeton Handbook for Reproducible Neuroimaging¶](https://brainhack-princeton.github.io/handbook/index.html)
