# SAP-PYTHON

Guide to connect Python with SAP 

## Introduction:

Simple guide to establish a connection with SAP's system using python code and trying to fetch the SAP table contents by calling the Function Module RFC_READ_TABLE.
This has multiple purposes that go from fetching data to analyzing purposes.

## Requirements:

- To make the connection we'll need to be able to establish a connection to with the SAP system to install SAPNWRFC SDK and PyRFC on your machine.

- Must have admin rights to configure the build path.

## Download and installation:

*Note that the steps mentioned below is for Windows 10 OS 64-bit only.

### Python installation

#### 1. Go to python.org
#### 2. Hover the mouse on the 'Downloads' page in python.
#### 3. Go to  on ‘All releases’.
#### 4. Search for the latest release.
#### 5. Scroll down to the ‘Files’ section and select either ‘Windows x86-64 executable installer’ or ‘Windows x86-64 web-based installer’.
#### 6. The Python Installer will launch and follow the steps as mentioned in the installer. It´s very important to make sure to have the option 'add python 3.x to path' ticked.
#### 7. Once the installation completes, make sure that the version of python from the command prompt is the same as the one installed. Type the following instruction in the command prompt to see the version of the python installed:
```bash
  python --version
```

### SAP NWRFCSDK installation:

#### 1. Go to the website in the link below to download the NWRFCSDK 7.50 from SAP’s site. Please make sure to choose the right version to download.  Its important to have a S-user for this purpose and permissions to download the software. Please contact the administrator of your organization if you do not have one. 

[NWRFCSDK](https://launchpad.support.sap.com/#/softwarecenter/template/products/_APP=00200682500000001943&_EVENT=DISPHIER&HEADER=Y&FUNCTIONBAR=N&EVENT=TREE&NE=NAVIGATE&ENR=01200314690100002214&V=MAINT)
#### 2. Create a folder ‘nwrfcsdk’ in C:\

#### 3. Extract the contents of zip file in the path C:\nwrfcsdk

#### 4. You’ll see another nwrfcsdk folder inside C:\nwrfcsdk, cut and paste the contents from C:\nwrfcsdk\nwrfcsdk and move it to C:\nwrfcsdk folder.

#### 5. Go to build PATH simply typing ‘environment’ in the search option next to windows logo.

#### 6. Go to build PATH following the path as: enviroment variables -> System variables -> Search for 'Path' and click edit. Now you have to make sure the variables C:\nwrfcsdk\lib and C:\nwrfcsdk\bin are in the Path if not you must create them. (Just to make sure also check the python paths are correctly written).

### PyRFC & Cython installation:

#### 1. Make sure pip is installed in your python, type 'pip show pip'. If there is an error then you should install it following this guide: 
[Pip Install](https://pip.pypa.io/en/stable/installation/)

#### 2. To install Cython you need to run the following command in the cmd prompt:
```bash
  pip install cython
```

#### 3. Now for the installation of PyRFC you can type the command 'wget https://github.com/SAP/PyRFC/releases/download/2.0.0/pyrfc-2.0.0-cp38-cp38-win_amd64.whl' in the cmd prompt. If wget doesn't work then you can download PyRFC following the guide of installation in https://github.com/SAP/PyRFC.

#### 4. Now that the installation of PyRFC is complete you need to type  ‘from pyrfc import connection’ in the command prompt, if it runs properly then it will not throw any errors and move on to a new command line. If it does not then it will throw an error. Based on the error you need to debug the issue by searching it in a browser or looking it up on GitHub.

### Jupyter Notebook Installation:

#### 1. Type in the cmd prompt  ‘pip install jupyter’.

#### 2. Once the installation is complete type ‘jupyter notebook’ to open an internet screen with Jupyter Notebook.

#### 3. Now in Jupyter go to the dropdown option ‘New’ and select ‘Python 3’.

#### 4. It will open a new project screen. This is where we'll put the python code later.

### File nwrfcsdk
Now the final step is to go to C:\nwrfcsdk\bin and double-click on rfcexec.exe file and see if it runs properly. If it does then a pop-up command prompt will appear for a while and then disappear. This indicates that the installation was successful.

## Code Implementation





