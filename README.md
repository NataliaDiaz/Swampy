# Swampy

by Allen Downey

Swampy is a suite of Python programs that support the books [*Think Python*](http://greenteapress.com/thinkpython)
and [*The Little Book of Semaphores*](http://greenteapress.com/semaphores).

It includes the following modules:

* AmoebaWorld: a fun way for beginning programmers to practice writing
	     Python expressions.

* TurtleWorld: an implementation of turtle graphics used in *Think Python* (first edition)

* TurmiteWorld: an implementation of Langton's ant.

* Lumpy: a program that generates UML object and class diagrams from a
       Python program.

* Sync: a thread simulator for use with *The Little Book of Semaphores*.

A description of the project and documentation is available at (http://www.greenteapress.com/thinkpython/swampy)






## INSTALLATION: Python 3 recommended (display not working for now in Python 2):

http://web.archive.org/web/20080116080037/http://allendowney.com/ip04/hw02/hw02.html

STEPS REQUIRED ONLY FOR MAC:

Install pip if you dont have it via https://pip.pypa.io/en/stable/installing/#installing-with-get-pip-py

using python get-pip.py --user

Then add the following line

export PATH=/Users/nataliadiazrodriguez/Library/Python/2.7/bin:$PATH

To your bashrc file doing

Nano ~/.bashrc



STEPS:

a) If in Windows/mac: Create a new conda environment with python 3.6 if it is not the default in your machine (check your version running ‘python’ in the terminal):

conda create -n myenv python=3.6

Eg.: conda create -n swampy python=3.6

And install swampy and tkinter:

pip install swampy
pip install swampy --user


conda install -c anaconda tk

b) In Linux:
Replicate the environment by doing

cd Swampy/python3:

conda env create -f environment.yml





## Test the environment and play with it

Test the installation running python3/test.py or in the command line:

conda activate Swampy

(amoeba)$ python
Python 3.6.8 |Anaconda, Inc.| (default, Dec 30 2018, 01:22:34)
[GCC 7.3.0] on linux
Type "help", "copyright", "credits" or "license" for more information.
>>> from swampy.TurtleWorld import *
>>> w = TurtleWorld()
>>> w.mainloop()


Then follow the first sections of:
http://www.greenteapress.com/thinkpython/swampy/amoeba.html

http://www.greenteapress.com/thinkpython/swampy/tutorial.html

Note: broken link: http://www-gap.dcs.st-and.ac.uk/~history/Curves/Curves.html

http://www.greenteapress.com/thinkpython/swampy/amoeba.html

## Extras

You can save your working environment for your machine to later reproduce it by doing:

conda env export > environment.yml

and saving it in your github repo.
