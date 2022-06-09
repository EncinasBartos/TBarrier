# Installation

## Download this repository
To install this repository you can download [TBarrier](https://github.com/EncinasBartos/TBarrier.git), unzip it, rename the resulting directory to `TBarrier` and move it to your development directory.

## Install Anaconda
Next, you will need Python 3 and a bunch of Python libraries. The simplest way to install these is to [download and install Anaconda](https://www.anaconda.com/distribution/), which is a great cross-platform Python distribution for scientific computing. If you prefer a lighter weight Anaconda distribution, you can [install Miniconda](https://docs.conda.io/en/latest/miniconda.html), which contains the bare minimum to run the `conda` packaging tool. You should install the latest version of Anaconda (or Miniconda) available.

Once Anaconda (or Miniconda) is installed, run the following command to update the `conda` packaging tool to the latest version:

    $ conda update -n base -c defaults conda

> **Note**: if you don't like Anaconda for some reason, then you can install Python 3 and use pip to install the required libraries manually (this is not recommended, unless you really know what you are doing). I recommend using Python 3.7, since some libs don't support Python 3.8 or 3.9 yet.

## Create the `TBarrier` Environment
Next, make sure you're in the `TBarrier` directory and run the following command. It will create a new `conda` environment containing every library you will need to run all the notebooks (by default, the environment will be named `TBarrier`, but you can choose another name using the `-n` option):

    $ conda env create -f environment.yml

Next, activate the new environment (from the terminal):

    $ conda activate TBarrier

## Start Jupyter
It's almost done! You just need to register the `TBarrier` conda environment to Jupyter. The notebooks in this project will default to the environment named `python3`, so it's best to register this environment using the name `python3` (if you prefer to use another name, you will have to select it in the "Kernel > Change kernel..." menu in Jupyter every time you open a notebook):

    $ python3 -m ipykernel install --user --name=python3

And that's it! You can now start Jupyter like this:

    $ jupyter notebook

This should open up your browser, and you should see Jupyter's tree view, with the contents of the current directory. If your browser does not open automatically, visit [localhost:8888](http://localhost:8888/tree).

Congrats! You are now ready to learn how to extract transport barriers from velocity data!

When you're done with Jupyter, you can close it by typing Ctrl-C in the Terminal window where you started it. Every time you want to work on this project, you will need to open a Terminal, and run:

    $ cd Name-of-Directory $ # or whatever development directory you chose earlier
    $ cd TBarrier
    $ conda activate TBarrier
    $ jupyter notebook

## Update This Project and its Libraries
I regularly update the notebooks to fix issues and add support for new libraries. So make sure you update this project regularly.

For this, open a terminal, and run:

    $ cd Name-of-Directory # or whatever development directory you chose earlier
    $ cd TBarrier # go to this project's directory
    $ git pull

Next, let's update the libraries. First, let's update `conda` itself:

    $ conda update -c defaults -n base conda

Then we'll delete this project's `TBarrier` environment:

    $ conda activate base
    $ conda env remove -n TBarrier

And recreate the environment:

    $ conda env create -f environment.yml

Lastly, we reactivate the environment and start Jupyter:

    $ conda activate TBarrier
    $ jupyter notebook
