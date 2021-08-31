# *[Python - Packages](https://www.tutorialsteacher.com/python/python-package)*


We organize a large number of files in different folders and subfolders based on some criteria, so that we can find and manage them easily. In the same way, a package in Python takes the concept of the modular approach to next logical level. As you know, a module can contain multiple objects, such as classes, functions, etc. A package can contain one or more relevant modules. Physically, a package is actually a folder containing one or more module files.


Let's create a package named mypackage, using the following steps:
<l1>1.Create a new folder named D:\MyApp.</l1>
<l2>2.Inside MyApp, create a subfolder with the name 'mypackage'.</l2>
<l3>3.Create an empty __init__.py file in the mypackage folder.</l3>
<l4>4.Using a Python-aware editor like IDLE, create modules greet.py and functions.py.</l4>

That's it. We have created our package called mypackage. The following is a folder structure:

<br>

[![Package Folder Sturcture](https://www.tutorialsteacher.com/Content/images/python/package.png "Package Folder Sturcture")](https://www.tutorialsteacher.com/Content/images/python/package.png)

Package Folder Sturcture

</br>

## Importing a Module from a Package

Now, to test our package, navigate the command prompt to the MyApp folder and invoke the Python prompt from there.

Import the functions module from the mypackage package and call its power() function.

It is also possible to import specific functions from a module in the package.

## __init__.py

The package folder contains a special file called __init__.py, which stores the package's content. It serves two purposes:

1.The Python interpreter recognizes a folder as the package if it contains __init__.py file.

2.__init__.py exposes specified resources from its modules to be imported.

An empty __init__.py file makes all functions from the above modules available when this package is imported. Note that __init__.py is essential for the folder to be recognized by Python as a package. You can optionally define functions from individual modules to be made available.

<div class="card noteDiv">
            <div class="card-header">
                <span><span> <i class="fa fa-pencil-square-o"></i></span> Note:</span>
            </div>
            <div class="card-body">
                We shall also create another Python script in the <code>MyApp</code> folder and import the mypackage package in it. 
                It should be at the same level of the package to be imported.
            </div>
            </div>

The __init__.py file is normally kept empty. However, it can also be used to choose specific functions from modules in the package folder and make them available for import.

The specified functions can now be imported in the interpreter session or another executable script.

Create test.py in the MyApp folder to test mypackage.

Note that functions power() and SayHello() are imported from the package and not from their respective modules, as done earlier. 

## Install a Package Globally
Once a package is created, it can be installed for system-wide use by running the setup script. The script calls setup() function from the setuptools module.

Let's install mypackage for system-wide use by running a setup script.

Save the following code as setup.py in the parent folder MyApp. The script calls the setup() function from the setuptools module. The setup() function takes various arguments such as name, version, author, list of dependencies, etc. The zip_safe argument defines whether the package is installed in compressed mode or regular mode.











