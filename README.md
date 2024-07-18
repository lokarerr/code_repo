# How-Tos

## Run C++ on VS-Code
1. Download a windows compatible C++ Compile (for example MinGW for Windows 11)
2. Install it locally (I installed it here: C:\MinGW\bin)
3. Update the path in environament variables: In Search bar look for "Setup Environment Variables" -> Environment Varibles -> "Path" -> Edit -> New -> paste the installation path -> OK
4. Re-open VS-Code
5. Install C/C++ extensions package in VS-Code
6. Write a C++ program and run using the GUI button or Ctrl + Alt + N

## Install Python Environment
1. Download python version of your choice (OS compatible) and install
2. Create virtual environment (venv): ```<INSTALLATION_PATH>/bin/python3.7.4  -m venv <LOCAL_PATH_FOR_VIRTUAL_ENV>```
3. Activate the venv: ```source bin/activate.csh```
4. Install packages: ```pip install -r ./requirements.txt```
5. Contents of the requirements.txt are in <PACKAGE>==<VERSION> syntax as follows

        pip==24.0
        scikit-learn==0.24.2
        pandas==1.1.3
        notebook==6.1.4
        matplotlib==3.3.2
        joblib==0.13.2
        seaborn==0.11.0
6. Use in scripts: as ```#!<LOCAL_PATH_FOR_VIRTUAL_ENV>/python/bin/python3```
   
