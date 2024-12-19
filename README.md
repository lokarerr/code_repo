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
5. Contents of the requirements.txt are in PACKAGE==VERSION syntax as follows

        pip==24.0
        scikit-learn==0.24.2
        pandas==1.1.3
        notebook==6.1.4
        matplotlib==3.3.2
        joblib==0.13.2
        seaborn==0.11.0
6. Use in scripts: as ```#!<LOCAL_PATH_FOR_VIRTUAL_ENV>/python/bin/python3```
   
## Install Connect to Remote SSH Host via VS-Code
1. Linux: Connect to a VNC machine with enough resources
2. Linux: Update the proxy settings under $HOME/.cshrc.$USER
3. Windows-VS-code: Install Remote-SSH extension
4. Windows-VS-code: VSCode, File → Preferences → Settings → search for "Http:proxy" and copy the http proxy into the field
5. Windows-VS-code: hit ctrl+shift+p > "Remote-SSH: Open SSH Configuration File". Add this to your ssh config file C:\Users\<your_username>\.ssh\config
        Host host_name
            HostName <host_name>.<site>.domain.com
            User <username>
6. Linux: make symobolic links for ~/.vscode-server: ln -s <workarea>/.vscode-server  ~/.vscode-server
7. Windows: Open powershell and run ssh-keygen -t rsa [Hit Enter, no need of password]
8. Linux: Copy the text from C:/Users/<username>/.ssh/id_rsa.pub at the bottom of ~/.ssh/authorized_keys
9. Windows-VS-code: Restart VSCode and hit ctrl+shift+p > "Remote SSH: Connect to Host" > Choose Linux
10. Windows-VS-code: To update Host: Hit 'Bin' symbol on the connection terminal to stop connecting to existing server.
11. ctrl+shift+p > "Remote-SSH: Open SSH Configuration File" > Update the host details
12. ctrl+shift+p > "Remote SSH: Connect to Host" > Choose the new host
    
