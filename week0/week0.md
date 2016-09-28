## Introduction to Conda, Jupyter Notebooks, Python, and R

_Conda is an open source package management system and environment management system for installing multiple versions of software packages and their dependencies and switching easily between them. It works on Linux, OS X and Windows, and was created for Python programs but can package and distribute any software._ -- <http://conda.pydata.org/docs/>

First, install miniconda3: <http://conda.pydata.org/miniconda.html>

Then, create a conda environment. Let's make an environment for doing statistics that includes Python 3, Jupyter, scikit-bio, and R. See <https://www.continuum.io/blog/developer/jupyter-and-conda-r> for more about R installation.

```bash
conda create -n stats python=3 jupyter scikit-bio
source activate stats
conda install -c r r-essentials
```

We can deactivate and then activate the conda environment to see what that looks like.

```bash
source deactivate
source activate stats
```

Note: We can also make a Qiime environment using instructions at <http://qiime.org/install/install.html>. We have to make a separate environment for that with python=2.7 because Qiime is written in Python 2.

Now we can start working through the three notebooks. In addition to this markdown readme file and the three notebooks, the directory contains a data file that we'll use with Pandas in the second notebook.

```
week0.md
week0.1_python_basics.ipynb
week0.2_pandas_matplotlib.ipynb
week0.3_r_basics.ipynb
scripps_pier_20151110.csv
```

