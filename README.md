
# Setting up Python environments
Key concepts and tips are summarized here.

## python 2 vs 3
Python 2.7 has been the widely used version for a while. 
Now, it's safe to use Python 3 (3.5 or 3.6).

In our lab servers, both python 2 and 3 are installed.
You can (should) run python 3 by typing python3 instead of python.
```
python3
```



You can check the version of the python as follows.
```
python --version
```
On Ubuntu 16.04.3, it will be Python 2.7.12.
```
python3 --version
```
On Ubuntu 16.04.3, it will be Python 3.5.2.

## For OSX users
You can install python 3 (and all the other open-source packages) using Mac Port. 

1. Install Mac Port
2. Install pythone 3.
```bash 
sudo port install python3
```

Also, you can keep it updated using the following commands.
```bash
sudo port -v selfupdate
sudo port upgrade outdated
```

See https://www.macports.org for more details.



## virtual environment 
In pythone 3 (from 3.3), venv is the standard way for creating and using virtual environments.

See https://docs.python.org/3/library/venv.html for more information.


## pip
You can use 'pip' to install python modules.

See https://docs.python.org/3/installing/index.html?highlight=pip for more information.

It is quite tricky where the actual modules and librararies are installed. 

In the virtual environment, don't worry about it and just use pip without any options.
(This is another reason why virtual environment is useful and recommended.)
For example, you can install latest tensorflow as follows.
```bash
pip3 install --upgrade tensorflow
```
Here, I assume that you installed pip for python3 and it's name is pip.
You can do it by 
```bash
sudo apt install python3-pip
```

If you want to install some module for syetem-wide access, then you can do it in two ways.
1. If you have the admnistrator privilege, you can do something like this.
```bash
sudo pip3 install --upgrade tensorflow
```
But, you will face some warning that says ....

2. If you are not and admnistrator, you must install the modules under your home folder. 
```bash
pip3 install --user --upgrade tensorflow
```



## Jupyter notebook
Jupyter notebook (previously known as Ipython notebook) is a great tool for interactive data analysis. 
It is also great that you can do the actual computations on a server and control it through a web-brower on your local machine. 
See https://github.com/ys7yoo/tutorial_IPython for more information.


