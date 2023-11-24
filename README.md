# ipykernel-ctl

Easily deploy IPyKernel for Python Environments. Automatically deploy and manage IPyKernel instances. IPyKernel allows to run Python environments in Jupyter Lab and Notebook. Deploy a kernel while inside of an environment, to use that environment in Jupyter Lab and Notebook. Note that IPyKernel and Jupyter Lab should be installed on your user Python environment (only for data redundancy reasons).

## Requirements

Make sure the following PIP packages are installed on your base system outside of any virtual environments.
* `pip install ipykernel`
* `pip install jupyterlab` (unless you don't want to use this for Jupyter).
* Some virtual environment utility: `pip install pipenv`

# Installation

Install script either using `wget https://raw.githubusercontent.com/Yiannis128/ipykernel-ctl/master/ipykernel-ctl`. Place it in you `PATH`.

# Basic Commands and Workflow

## Initialize a Kernel

Generally, you enter a virtual environment, go to your project folder, and run the following command:

```sh
ipykernel-ctl --create
```

This will create a new kernel and give it a unique name based off your folder and path (much like pipenv).

## List Kernels

You can use the following command to list all currently initialized kernels:

```sh
ipykernel-ctl --list
```

## Delete a Kernel

You can use the following command to delete the kernel associated with the folder you are currently inside of:

```sh
ipykernel-ctl --delete
```

You can also pass it a kernel name to delete a specific one:

```sh
ipykernel-ctl --delete mykernel-abcd
```

# Contributions

Please create issues to request any features that you would like added. You can then fork the repository, make additions, and create a pull request. Alternatively, you can wait for it to be implemented _at some point_ :)
