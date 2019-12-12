# TV Script Project Overview

The TV Script Generation project is the third project of the Udacity Deep Learning Nano Degree. The project consists of using a Recurrent Neural Network (RNN) to generate a TV script. The RNN is trained on an existing scripts, then used to generate an original piece of writing.

# Instruction 

1. Clone the repository
```console
git clone https://github.com/atkatchev/tv_script_generation.git
```
2. Conda users follow below or see [Dependencies Section](#Dependencies)
```console 
conda create -n deep-learning python=3.6
source activate deep-learning
conda install pytorch torchvision -c pytorch 
pip install -r requirements.txt 
```
3. Open the project file using jupyter notebook. Otherwise, open .html page
```console
jupyter notebook dlnd_tv_script_generation.ipynb
``` 

# Project Structure

* dlnd_tv_script_generation.ipynb: Notebook of the project
* dlnd_tv_script_generation.html: HTML version of the Notebook
* generated_script_1.txt: generated script 
* helper.py: helper functions to pre-process data and saving and loading the model 
* problem_unittests.py: Test file validating TODO functions in the projectd
* [dataset](https://www.kaggle.com/thec03u5/seinfeld-chronicles#scripts.csv)

# Contents

* Pre-processed Data
* Define the Models
* Optimizers
* Training
* Training Loss

# Dependencies

## Configure and Manage Your Environment with Anaconda

Per the Anaconda [docs](http://conda.pydata.org/docs):

> Conda is an open source package management system and environment management system 
for installing multiple versions of software packages and their dependencies and 
switching easily between them. It works on Linux, OS X and Windows, and was created 
for Python programs but can package and distribute any software.

## Overview
Using Anaconda consists of the following:

1. Install [`miniconda`](http://conda.pydata.org/miniconda.html) on your computer, by selecting the latest Python version for your operating system. If you already have `conda` or `miniconda` installed, you should be able to skip this step and move on to step 2.
2. Create and activate * a new `conda` [environment](http://conda.pydata.org/docs/using/envs.html).

---

## 1. Installation

**Download** the latest version of `miniconda` that matches your system.

|        | Linux | Mac | Windows | 
|--------|-------|-----|---------|
| 64-bit | [64-bit (bash installer)][lin64] | [64-bit (bash installer)][mac64] | [64-bit (exe installer)][win64]
| 32-bit | [32-bit (bash installer)][lin32] |  | [32-bit (exe installer)][win32]

[win64]: https://repo.continuum.io/miniconda/Miniconda3-latest-Windows-x86_64.exe
[win32]: https://repo.continuum.io/miniconda/Miniconda3-latest-Windows-x86.exe
[mac64]: https://repo.continuum.io/miniconda/Miniconda3-latest-MacOSX-x86_64.sh
[lin64]: https://repo.continuum.io/miniconda/Miniconda3-latest-Linux-x86_64.sh
[lin32]: https://repo.continuum.io/miniconda/Miniconda3-latest-Linux-x86.sh

**Install** [miniconda](http://conda.pydata.org/miniconda.html) on your machine. Detailed instructions:

- **Linux:** http://conda.pydata.org/docs/install/quick.html#linux-miniconda-install
- **Mac:** http://conda.pydata.org/docs/install/quick.html#os-x-miniconda-install
- **Windows:** http://conda.pydata.org/docs/install/quick.html#windows-miniconda-install

## 2. Create and Activate the Environment

For Windows users, these following commands need to be executed from the **Anaconda prompt** as opposed to a Windows terminal window. For Mac, a normal terminal window will work. 

#### Git and version control
These instructions also assume you have `git` installed for working with Github from a terminal window, but if you do not, you can download that first with the command:
```
conda install git
```

**Now, were ready to create our local environment!**

1. Clone the repository, and navigate to the downloaded folder. This may take a minute or two to clone due to the included image data.
```
git clone https://github.com/udacity/deep-learning-v2-pytorch/tree/master/project-bikesharing
cd project-bikesharing
```

2. Create (and activate) a new environment, named `deep-learning` with Python 3.6. If prompted to proceed with the install `(Proceed [y]/n)` type y.

    - __Linux__ or __Mac__: 
    ```
    conda create -n deep-learning python=3.6
    source activate deep-learning
    ```
    - __Windows__: 
    ```
    conda create --name deep-learning python=3.6
    activate deep-learning
    ```
    
    At this point your command line should look something like: `(deep-learning) <User>:deep-learning-v2-pytorch <user>$`. The `(deep-learning)` indicates that your environment has been activated, and you can proceed with further package installations.

3. Install PyTorch and torchvision; this should install the latest version of PyTorch.
    
    - __Linux__ or __Mac__: 
    ```
    conda install pytorch torchvision -c pytorch 
    ```
    - __Windows__: 
    ```
    conda install pytorch -c pytorch
    pip install torchvision
    ```

6. Install a few required pip packages, which are specified in the requirements text file (including OpenCV).
```
pip install -r requirements.txt
```

7. Thats it!

Now, assuming your `deep-learning` environment is still activated, you can navigate to the main repo and start looking at the notebooks:

```
cd
cd deep-learning-v2-pytorch
jupyter notebook
```

To exit the environment when you have completed your work session, simply close the terminal window.
