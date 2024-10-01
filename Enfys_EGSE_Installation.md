# .github

Enfys General EGSE initialisation : 01/10/2024
Prerequisites : 
1.  Git
   -----
     Install git from : https://github.com/git-for-windows/git/releases/download/v2.46.2.windows.1/Git-2.46.2-64-bit.exe
   
2.  AMD Vivado
   -----------
    1. To instal AMD Vivado, first create an AMD account (essential as you need it to initialise the program).
    2. Then navigate to : https://www.xilinx.com/member/forms/download/xef.html?filename=FPGAs_AdaptiveSoCs_Unified_2024.1_0522_2023_Win64.exe to download the 64 bit Windows variant.
    3. Complete the U.S Export approval form.
    4. Go through the installation process. When you get prompted what software to install you only need the A7 variants, deselect all other and Vitis.
    
3.  VSCode
   -------
     Install VsCode from : https://code.visualstudio.com/
   
4.  Python 3.12
   ------------
     Install Python from the Python foundation : https://www.python.org/downloads/
     Follow the installer instructions for python, ensure the following options are enabled:
    - Add python to the system path
    - Disable the path length limit
    Once python has finished installing verify correct configuration by opening a powershell terminal and typing `python`. If correctly installed then a few lines should appear with the first line stating `Python 3.10.2...` or whatever version was installed. Exit the python terminal by simply typing `exit()`.
     
5.  Poetry
    ------
        Next install pypoetry, the current [reccomended way](https://python-poetry.org/docs/#windows-powershell-install-instructions) is to simply open up a powershell terminal and type the following. It's worth checking the link to ensure this hasn't changed:

      ```PowerShell
        (Invoke-WebRequest -Uri https://raw.githubusercontent.com/python-poetry/poetry/master/get-poetry.py -UseBasicParsing).Content | python -
      ```
         Once pypoetry has been installed verify it too has been successfully installed by simply typing `poetry` within a powershell terminal. If it is correctly installed then the first line should print the version `Poetry version 1.1.13` followed by the command line options.
6.  Labview 2022.1
    ---------------
        Install LabView from the Labview website
     
7.  enfys_fw repo rebuild branch
    -----------------------------
        Clone the firmware repository - rebuild branch from : https://github.com/ExoMars-Enfys/enfys_fw.git
        To Regenerate project:
        Open Vivado
        In Tcl console, cd to proj directory
        Type    source <tcl filename>.tcl        
        The project will be regenerated
        Note: this project has no build files. To build the project again click Generate bitstream
 
    
9.  Python Uart_Lib Repo UI_Lib_V2 Branch
   --------------------------------------
       Clone the Python_Uart_Lib repository - UI_LIB_V2 branch from : https://github.com/ExoMars-Enfys/Python_UART_Lib
       Within the vscode terminal simply type `poetry install`. This will create a new folder `.venv` within the project folder and automatically download and install `vsg` into the python environment. This folder will not be committed to the repo but simply contain the python virtual environment with any installed libraries.

     
  
