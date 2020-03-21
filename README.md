# install-Anaconda-jupyter-notebook-with-tensor-flow-and-kersa
First of all we need to install Anaconda and then using conda environment we will install tensorflow with keras for machine learning.
For installing Anaconda
follow the steps.
step 1 - $ download the newest version of conda from it official website. link is given below
$ https://www.anaconda.com/download/#macos
step 2 -from here you will get .sh file 
go to the folder where .sh file is available. Open the terminal in that folder by right clicking the mouse button.
then write the command $ ls
and see the conda installation file.
copy the file name with extension .sh, then type on terminal ./install filename.sh
use can use sudo if you are getting permission problem
$ ./install Anaconda3-2020.02-Linux-x86_64.sh
or
$ sudo ./install Anaconda3-2020.02-Linux-x86_64.sh

then the process of installation of Anaconda will start and you need to follow the step whatever coming on screen.

Once conda will install then update conda in your default environment
$ conda upgrade conda

you can check the default virtual environment by using command
$ conda info -e
then you will see the existing virtual environment.
you can install tensorflow in that default environment by using the command
$ conda install tensorflow
and now you can check it.
$ python
>>> import tensorflow as tf
>>> print(tf.__version__)
>>> import tf.keras

Now you have jupyter notebook together with tensorflow and keras
enjoy machine learning algorithms.



2- you can create other virtual environment by using command
$ conda create -n filename     #file name you can write by your own
$ conda activate filename

take look of environmaent you have created
$ conda info
$ conda list

if you want see currently virtual environment which you have created
$ conda info -e

when you want come out from any enivronment 
$ conda deactivate

and if you want to remove any virtual environment
$ conda env remove --name filename


Now conda verse pip
both are open source package managers. you can install virtual environment using both of them.
using conda install you can install any package software
and using pip install you will install only python packages


We can install tensorflow using pip alos.
first we need to create a virtual environment 
$ conda create -n tf_2                    # tf_2 is the environment name you can choose according to your wish
$ conda activate tf_2
(tf_2)gaurav@gaurav-Veriton-M2640G:~$ 
now first install pip in virtual environment
$ conda install pip

# Install tensorflow cpu version using pip
$ pip install --upgrade tensorflow    # for python2
$ pip3 install --upgrade tensorflow   # for python3

#now install keras (note first install tensorflow)
pip install keras

and then check againg
by typing python
$ python
>>> import tensorflow as tf
>>> print(tf.__version__)

Done
