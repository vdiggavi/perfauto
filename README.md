# perfauto
performance test automation using locust.io

## Installation

* install VS Code (straightforward installation)
* install python 3.11.1 for windows. Note the following options:
  * Check 'add python to path' while installing
  * typical install
  * enable path lengths over 260 characters.
  * when installation is finished, do this basic check: in a cmd-prompt type "python". This should start the python. Exit with CTRL+Z
* GIT (#TODO)
  * Use a GIT client (git bash, sourcetree or any other of your choice)
  * create a folder for your python projects
  * in that folder, clone the git-repo. In git bash it is this command: #TODO

* in VS Code:
  * File -> Open Folder and open your automation folder
  * install python extension (click on extension icon (the square on the left pane), search for python and install). Then restart VS CODE.
  * In VS Code go to the terminal and create a virtual environment:
    >python -m venv env
  * This creates a folder "env" in the project folder (it's ignored by git)
  * activate your new virtual environment:
    >env\scripts\activate

    * Note:
      On Microsoft Windows, it may be required to enable the Activate.ps1 script by setting the execution policy for the user. You can do this by issuing the following PowerShell command:
      >PS C:> Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
  * To install and validate dependencies cd to root directory (Ex: cd D:\Automation) and run the following:
    >pip3 install locust
    >locust -V
  * Done
  * IMPORTANT: whenever you start working on this project, the first thing you do is activate your virtual environment:  
    * either with the command CTRL+SHIFT+P (Python: create terminal) it will automatically find your virtual environment and activate it
    * either manually in the terminal: env\scripts\activate

## Automated performance tests using Locust tool
What is Locust?
Locust is an easy to use, scriptable and scalable performance testing tool.
You define the behaviour of your users in regular Python code, instead of being stuck in a UI or restrictive domain specific language.
This makes Locust infinitely expandable and very developer friendly.

## Running Performance tests

Change directory to locustfiles in both (Example: cd D:\Automation\LoadTests> )

- To Run all scenarios enter locust in the terminal:
  >`locust`
- Browse <http://localhost:8089>
