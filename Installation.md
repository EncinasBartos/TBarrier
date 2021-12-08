# Installation

## Download this repository
To install this repository and run the Jupyter notebooks on your machine, you will first need git, which you may already have. Open a terminal and type `git` to check. If you do not have git, you can download it from [git-scm.com](https://git-scm.com/).

Next, clone this repository by opening a terminal and typing the following commands (do not type the first `$` on each line, it's just a convention to show that this is a terminal prompt, not something else like Python code):

    $ cd $HOME  # or any other development directory you prefer
    $ git clone https://github.com/EncinasBartos/TBarrier.git
    $ cd TBarrier

If you do not want to install git, you can instead download the zip file by going to [TBarrier](https://github.com/EncinasBartos/TBarrier) --> Code --> unzip, rename the resulting directory to `TBarrier` and move it to your development directory.

## Install Anaconda
Next, you will need Python 3 and a bunch of Python libraries. The simplest way to install these is to [download and install Anaconda](https://www.anaconda.com/distribution/), which is a great cross-platform Python distribution for scientific computing. It comes bundled with many scientific libraries, including NumPy, Pandas, Matplotlib, Scikit-Learn and much more, so it's quite a large installation. If you prefer a lighter weight Anaconda distribution, you can [install Miniconda](https://docs.conda.io/en/latest/miniconda.html), which contains the bare minimum to run the `conda` packaging tool. You should install the latest version of Anaconda (or Miniconda) available.

During the installation on MacOSX and Linux, you will be asked whether to initialize Anaconda by running `conda init`: you should accept, as it will update your shell script to ensure that `conda` is available whenever you open a terminal. After the installation, you must close your terminal and open a new one for the changes to take effect.

During the installation on Windows, you will be asked whether you want the installer to update the `PATH` environment variable. This is not recommended as it may interfere with other software. Instead, after the installation you should open the Start Menu and launch an Anaconda Shell whenever you want to use Anaconda.

Once Anaconda (or Miniconda) is installed, run the following command to update the `conda` packaging tool to the latest version:

    $ conda update -n base -c defaults conda

> **Note**: if you don't like Anaconda for some reason, then you can install Python 3 and use pip to install the required libraries manually (this is not recommended, unless you really know what you are doing). I recommend using Python 3.7, since some libs don't support Python 3.8 or 3.9 yet.

## Create the `TBarrier` Environment
Next, make sure you're in the `TBarrier` directory and run the following command. It will create a new `conda` environment containing the libraries needed to run all the notebooks:

    $ conda create -n TBarrier -c conda-forge --file requirements.txt
   
When doing so, the libraries installed through pip are not installed into the conda environment. They thus have to be added manually via "pip install <name_of_library>"    
Alternatively we recommend installing the required packages from the yml file:

    $ conda env create -f environment.yml

Next, activate the new environment (from the terminal):

    $ conda activate TBarrier

## Start Jupyter
It's almost done! You just need to register the `TBarrier` conda environment to Jupyter. The notebooks in this project will default to the environment named `python3`, so it's best to register this environment using the name `python3` (if you prefer to use another name, you will have to select it in the "Kernel > Change kernel..." menu in Jupyter every time you open a notebook):

    $ python3 -m ipykernel install --user --name=python3

And that's it! You can now start Jupyter like this:

    $ jupyter notebook

This should open up your browser, and you should see Jupyter's tree view, with the contents of the current directory. If your browser does not open automatically, visit [localhost:8888](http://localhost:8888/tree). Click on `index.ipynb` to get started.

Congrats! You are now ready to learn how to extract transport barriers from velocity data!

When you're done with Jupyter, you can close it by typing Ctrl-C in the Terminal window where you started it. Every time you want to work on this project, you will need to open a Terminal, and run:

    $ cd Name-of-Directory $ # or whatever development directory you chose earlier
    $ cd TBarrier
    $ conda activate TBarrier
    $ jupyter notebook

## Update This Project and its Libraries
I regularly update the notebooks to fix issues and add support for new libraries. So make sure you check out this repository regularly.
