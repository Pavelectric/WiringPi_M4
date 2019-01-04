## What's so interesting - here is a description and some files for working with GPIO I / O on the M4 card.

#### So ... installing tools for working with GPIO has two ways:
1. If you use to work Python 2.
2. If you use to work Python 3.

#### By default I will talk about Python3, and for Python2 I will make special notes.

### To work correctly, you need the following packages (install them):

```$ sudo apt-get install git python-dev python-setuptools python3-dev python3-setuptools swig```

### Next, you need the file "setuptools-33.1.1.zip", it is here in the folder. 
Unpack it with a team (at your discretion):

```$ unzip setuptools-33.1.1.zip```

### Next, go to the folder with the unpacked arching:

```$ cd setuptools-33.1.1```

### And install the package with the command:

``$ sudo python3 setup.py install``

(If you are using Python2 - ```$ sudo python2 setup.py install```)

### Now we proceed to the installation of WiringPi itself:

```$ sudo easy_install wiringpi-2.44.4-py3.6-linux-aarch64.egg```

(If you are using Python2 - ```$ sudo easy_install-2.7 wiringpi-2.44.4-py2.7-linux-aarch64.egg```)

### After the installation is complete, check and execute the command:

```$ gpio readall```

### You should get a table in the terminal window, in which GPIO parameters are specified with reference to physical pins.
Example table:

![alt text](https://github.com/Pavelectric/M4/blob/master/M4_Readall.png)

Files and materials from the following source are used:
[wiki.friendlyarm](http://wiki.friendlyarm.com/wiki/index.php/WiringPi-Python_for_RK3399/zh)
