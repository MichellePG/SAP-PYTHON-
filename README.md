# SAP-PYTHON

Guide to connect Python with SAP 

## Introduction:

Simple guide to establish a connection with SAP's system using python code and trying to fetch the SAP table contents by calling the Function Module RFC_READ_TABLE.
This has multiple purposes that go from fetching data to analyzing purposes.

## Requirements:

To make the connection we'll need to be able to establish a connection to with the SAP system to install SAPNWRFC SDK and PyRFC on your machine.

Must have admin rights to configure the build path.

## Download and installation:

*Note that the steps mentioned below is for Windows 10 OS 64-bit only.

### Python installation

#### 1. 
Go to python.org
#### 2. 
Hover the mouse on the 'Downloads' page in python.
#### 3. 
Go to  on ‘All releases’.
#### 4. 
Search for the latest release.
#### 5.
Scroll down to the ‘Files’ section and select either ‘Windows x86-64 executable installer’ or ‘Windows x86-64 web-based installer’.
#### 6. 
The Python Installer will launch and follow the steps as mentioned in the installer. It´s very important to make sure to have the option 'add python 3.x to path' ticked.
#### 7.
Once the installation completes, make sure that the version of python from the command prompt is the same as the one installed. Type the following instruction in the command prompt to see the version of the python installed:
```bash
  python –version
```

### SAP NWRFCSDK installation:

#### 1.
Go to the website in the link below to download the NWRFCSDK 7.50 from SAP’s site. Please make sure to choose the right version to download.  Its important to have a S-user for this purpose and permissions to download the software. Please contact the administrator of your organization if you do not have one. 

[Documentation](https://launchpad.support.sap.com/#/softwarecenter/template/products/_APP=00200682500000001943&_EVENT=DISPHIER&HEADER=Y&FUNCTIONBAR=N&EVENT=TREE&NE=NAVIGATE&ENR=01200314690100002214&V=MAINT)
#### 2. 
Create a folder ‘nwrfcsdk’ in C:\

#### 3.
Extract the contents of zip file in the path C:\nwrfcsdk

#### 4. 
You’ll see another nwrfcsdk folder inside C:\nwrfcsdk, cut and paste the contents from C:\nwrfcsdk\nwrfcsdk and move it to C:\nwrfcsdk folder.

#### 5.
