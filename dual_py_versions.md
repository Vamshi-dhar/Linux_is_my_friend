### Create a New Environment
`<conda create --name subscribe python=3.6>`

### You can also create an environment with multiple packages in it. This also gives you the option to install additional packages later if you need them.
`<conda create --name chooseAnotherName python=3.6 numpy pandas scipy>`

### Enter an Environment
`<source activate subscribe>`

### Leave an Environment
`<source deactivate subscribe>`

### List your Environments
`<conda env list>`

### Remove an Environment
`<conda env remove --name subscribe>`

# Using Both Python 2.x and Python 3.x Environments in IPython Notebook

### Open a new terminal and check your conda version by typing
`<conda --version>`

if you are below anaconda 4.1.0, type conda update conda


### Next we check to see if we have the library nb_conda_kernels by typing
`<conda list>`

### If you don’t see nb_conda_kernels type
`<conda install nb_conda_kernels>`

### If you are using Python 2 and want a separate Python 3 environment please type the following
`<conda create -n <py36> python=3.6 ipykernel>`

### If you are using Python 3 and want a separate Python 2 environment, you could type the following.
conda create -n <py27> python=2.7 ipykernel

Close your terminal and open up a new terminal. type jupyter notebook
Click new and you will see your virtual environment listed.
