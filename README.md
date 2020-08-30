# Setting up Environments and Installing Packages Using Conda

## Summary of steps to complete

- [ ] Fork this repository so you have your own copy to work on.
- [ ] Clone the repository on your local machine. 
- [ ] Edit this README.md file on your machine.
- [ ] Run the Conda commands shown in the video and describe them in the table below.
- [ ] Push your changes to your GitHub repository.
- [ ] Submit a link to this GitHub repository in Canvas.

## 1. Fork & Clone this repository

* We did this in a previous assignment. Instructions are here: https://github.com/cmcntsh/N6806_Fall2020_DevNotes/blob/master/Projects/002%20-%20Practice%20Using%20Git%20and%20GitHub/README.md
* This can also be done directly in VSCode
  * Create a new folder on your machine where you want to put this repository if you don't already have one you want to use.
  * Copy the Clone or Download path for this repository from GitHub.
  * In VSCode from the command pallette (Ctrl-Shift-P) run Git: Clone
  * Paste the path into the path field which pops up
  * Select your new folder you created on your machine
  * A new folder for the repository with the repository files should be in the folder you selected showing in the Explorer window in VSCode on the left side.
  
## Edit your README.md file

* [ ] In an editor of your choice (i.e. VSCode) edit this README.md file to add the answers requested in the tables.

## Follow along with this tutorial

* Conda What and Why? (27 min): https://www.youtube.com/watch?v=23aQdrS58e0&list=PLG9A6ovzPqX6d9uWzx0UYN9pm0zzl5ofA&index=13&t=0s
  * He installs Miniconda. We will be using Anaconda. Don't install Miniconda.
  * Follow along with the rest of the tutorial.
  * Go ahead and create the environments as he creates them in the tutorial.

## Conda Concepts

* [ ] Describe the Conda concepts used in the video and listed in the table below.

|   Concept   |         Description or short answer         |
|     ---     |                     ---                     |
|What is the purpose of having different environments?     |Each environment is for different projects and python applications|
|What is the default package manager in Python?            |pip, python's integrated package manager|
|How do you manage environments and packages in Anaconda?  |Virutalenv or Conda|
|`conda list`       |all the default packages included and installed with anaconda, long list|
|`conda env list`       |a list of the environments we have installed|
|How do you keep your base environment unchanged?       |by creating new environments in which to house new packages|
|What is the link to the Conda cheat sheet? (link in video notes is broken)      |https://docs.conda.io/projects/conda/en/4.6.0/_downloads/52a95608c49671267e40c689e0bc00ca/conda-cheatsheet.pdf|
|`conda create --name XXXX`       |to create and name a new environment|
|`source activate XXXX`       |this activates and lets you to be able to work within a specific env|
|`conda install YYYY`       |this installs packages that are not there by default|
|channels in Conda       |the location where Conda looks for the packages you want to install|
|`conda install -c ZZZZ YYYY`       |this installs packages from a specific channel, one time|
|`conda config --show channels`       |shows the channels you have|
|`conda config --add channels ZZZZ`       |add channels to be available by default in Conda|
|conda-forge.org       |a channel of python packages that is a community led collection|
|`source deactivate`       |brings you back to base channel|
|`conda config --get channels`       |you can see the priority of the channels|

* After creating the environments he created in the video on your computer, what would the results of running the command `conda env list` look like with the da35 environment activated. Paste the output from your command prompt in the code block below.

```
(da35) Macintosh:da35 genniferrubin$ conda list
# packages in environment at /Users/genniferrubin/opt/anaconda3/envs/da35:
#
# Name                    Version                   Build  Channel
ca-certificates           2020.7.22                     0  
certifi                   2018.8.24                py35_1  
libcxx                    10.0.0                        1  
libedit                   3.1.20191231         h1de35cc_1  
libffi                    3.2.1                h0a44026_6  
ncurses                   6.2                  h0a44026_1  
openssl                   1.0.2u               h1de35cc_0  
pip                       10.0.1                   py35_0  
python                    3.5.6                hc167b69_0  
readline                  7.0                  h1de35cc_5  
setuptools                40.2.0                   py35_0  
sqlite                    3.33.0               hffcf06c_0  
tk                        8.6.10               hb0a8c7a_0  
wheel                     0.35.1                     py_0  
xz                        5.2.5                h1de35cc_0  
zlib                      1.2.11               h1de35cc_3  
(da35) Macintosh:da35 genniferrubin$ 



```
* What command would you use to remove the environments you created for this exercise from your computer?

```
conda env remove --name [env name]

```
