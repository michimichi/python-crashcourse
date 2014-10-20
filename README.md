#python-crashcourse

The purpose of this repository is to provide a quick introduction into scientific computing with python for novices. 

## Setting up the environment
For now, we work with Python 2.7, since not all of the special libraries that we use have been ported to Python 3 yet.

    Make sure that you have Python 2.7 installed on your system. 

In order to decouple our working environment from the system it runs on, we use a so-called **virtual environment**.  [Google is your friend here.](https://www.google.de/webhp?sourceid=chrome-instant&ion=1&espv=2&ie=UTF-8#q=python%20virtualenv)

    Install virtualenv on your system. This is presumably the last package for this introduction that you have to install system-wide.
    
Create a virtual environment (how you do that, and in which place, is up to you). On a linux system, this looks like:
```{bash}
user@host:~/home/sandbox$virtualenv --no-site-packages env
New python executable in env/bin/python
Installing setuptools, pip...done.
user@host:~/home/sandbox$ 
```
This creates a virtual environment named `env` in the  directory /home/sandbox. This virtual environment needs to be activated:
```
user@host:~/home/sandbox$ source env/bin/activate
```
The shell prompt changes to indicate that the environment is active:
```
(env)user@host:~/home/sandbox$ 
```

From now on, you can easily install packages into the virtual environment without affecting the host system.
To conclude this section, install [numpy](http://www.numpy.org/) into the virtual environment. Numpy is a  package that is fundamental for scientific computing.
```
(env)user@host:~/home/sandbox$ pip install numpy
```
To leave the virtual environment, simply deactivate it:
```
(env)user@host:~/home/sandbox$ deactivate 
```

### Homework

Before we take some first steps in numpy in the next section, please take some time to familiarize yourself with git and github. In particular, please clone this repository on your machine - preferably into the directory in which you have installed the virtual environment (`in this case, /home/sandbox/`).
In upcoming commits, this repository will be updated with project files and assignments.


## First steps in numpy

Make sure that your virtualenv is activated and that numpy is installed. 

The file 'distributions.csv' contains a large number of samples from three different distributions.
Load this file with numpy, and plot the three distributions (Hint: matplotlib!)

Calculate mean values and standard deviations of each of these distributions and compare.

Why is the standard deviation of the third distribution a poor measure for the width? What would be a better estimate?



