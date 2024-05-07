# testing_README
Support material for [A Deep Dive into the Tennis Racket Paradox: Analysis and Numerical Simulations of the Intermediate Axis Theorem.](https://www.google.com/)



## Creating a Python virtual enviroment to run the scripts

If you have `virtualenv` 'virtualenv' installed, you can configure an isoleted Python enviroment to run the scripts of the repository.

Also the repository provides a 'virtualenv_requirements.txt' file to facilitate the installation of the dependencies.

'''
~$ mkdir virtualenvs
~$cd virtualenvs
~/virtualenvs$ virtualenv --python=python2.7 dzhanibekovEffect
'''

The virtual enviroment is created using `python2.7' which is the version of python neccesary for runnnign the scripts.

Once the virtual enviroment is created, it needs to be activated:

`~/virtualenvs$ source dzhanibekovEffect/bin/activate'

The name of the current virtual environment will now appear on the left of the prompt to let you know that it’s active. From now on, any package that you install using pip will be placed in the `dzhanibekovEffect' folder, isolated from the global Python installation.

We need to make sure that the pip version contained in the virtual environment is up to date

`$ pip install -U pip'

Now download the file `requirements.txt' and the `*.py' scripts and place them in the current folder. Then, we can install the required dependencies:

`~/virtualenvs$ pip install -r requirements.txt'

The main script is `test.py' and to execute it

`$python test.py'

Poner como se dá cuenta que termina OK

Once you are done working in the virtual environment for the moment, you can deactivate it:

`$ deactivate'

Now running python will just use the system’s default Python interpreter, which is not modified by anything done while being inside the virtual environment.

To delete a virtual environment, just delete the corresponding folder. (In this case, it would be rm -r dzhanibekovEffect).
