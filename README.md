# Python-for-Epidemiologists
/*READ THIS ENTIRE SECTION BEFORE DOWNLOADING*/
This is a guided tutorial for epidemiologists who are interested in using Python 3.x as a software for data cleaning/analysis. This tutorial is meant to provide the basics of coding in Python.
First, we will go over how to install and set up Python for the tutorial
In the tutorial, we will discuss: 
    1) Basics of Python 
    2) Data manipulation basics
    3) Epidemiology analysis tools
    4) Basic graphic creation

# Installing Python
To install, Python 3.x, we can download it directly from: https://www.python.org/downloads/
The installer provides an option to add Python3 to PATH, it is **highly recommended** you do this, since it allows you to avoid having to do the following part. However, installing Python from Rodeo for Windows users might necessitate the following.
Once downloaded, an environmental variable needs to be created for Python. We do this by (Windows 8/10):
    1. Open the Control Panel
    2. Select System
    3. Select Advanced system settings
    4. Select Environmental Variable
    5. Select Path in the User Variables for ______ section
    6. Add the file path of the Python install file (note that your install will likely differ from my example below, but last two path items should be very similar)
        Ex) C:\file\path\to\Python\Python35-32\
    7. Select OK
    8. Select OK
    9. Select Apply

## IDE (Integrated Development Environment)
This can be chosen later. I prefer to use Rodeo from Y-Hat, but any IDE will work. Basically what works/looks the best for you is what you should use. Some general options: Rodeo, Spyder, PyCharm, Jupyter Notebook (more in depth discussion here: https://www.datacamp.com/community/tutorials/data-science-python-ide)

You can download Rodeo from: https://www.yhat.com/products/rodeo
Also note that their blog (y-hat) has some good tutorials
Note that if using the Rodeo IDE for Windows, it downloads with copy of Python 3.x. As a result, Windows users only need to download Rodeo and then set their environmental variable. However, Mac users downloading Rodeo will need to download a copy of Python 3.x from the provided URL regardless.

## Installing Python Packages
Packages are what stores Python functions that we will use. These packages are contributed by various members of the community and there is a wide array. To be able to download packages, we need to make sure we have an environmental variable created for python. Below we will separate this into two section; Windows and Mac. We will discuss how to install packages for both
### Windows
Open Command Prompt. When opened, type 'python' and this should open Python in the same window. From here, you can quit by typing 'quit()' or closing the window. If this does NOT work, make sure your environmental variable was created properly
Python 3.x conveniently comes with a package manager. Basically it stores all the packages and we can use it to download new ones or update already downloaded ones.
To download a new package: Open Command Prompt and use the following code (we will be installing pandas)
```
python -m pip install pandas
```
Which will download our package and install it. If an error is output, I recommend googling it first for potential solutions. A common issue is that there is not a C compiler. One can be downloaded from Windows. An alternative is to download a .whl file of the package from: https://www.lfd.uci.edu/~gohlke/pythonlibs/
/*Make sure that the bit (32 or 64) of the WHL files matches the version of Python 3.x used*/
The .whl file can used to install the package from Command Prompt (after navigating to the folder containing the .whl file) through the following code
```
python -m pip install whlfilename.whl
```
/*Reminder, you can navigate to folders in Command prompt by*/
```
cd folder_name
```
To update a Python package, type the following command into Command Prompt. For example, we will update our pandas package
```
python -m pip install pandas --upgrade
```
Those are the basics of installing packages. Sometimes packages on Windows can be difficult to install. If having difficulties, .whl file is often an easy workaround. Afterwards, update the package using the above code.
### Mac
Verifying process...

### Required packages for tutorial
To complete the tutorial, user must have the following packages installed: numpy, pandas, networkx, zepid, matplotlib, statsmodels, sas7bdat
It is recommended to try install each using the above instructions

#### Recommended packages
Some other useful packages: seaborn (improved graphical outputs), biopython (bunch of useful functions, but can search PubMed)

# Tutorial Parts
## 1. Python Basics
python_basics.md
python_basics.txt
## 2. Data manipulation basics
data_basics.md
data_basics.txt
## 3. Epidemiologic analysis
under development
## 4. Basic graphic creation
under development
