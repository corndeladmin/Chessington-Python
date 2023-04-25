# Chessington

1. Fork this repo: click `Fork` in the top-right of the page - this will create a copy of this repo in **your own GitHub account**

2. Clone (download) the repo
    * Go to your newly-created fork of the repo (on GitHub).
    * Click `Clone or download` (the green button on the right).
    * Make sure the page says `Clone with SSH` (rather than `Clone with HTTPS`).
    * Open your git client (e.g. GitKraken) and use this link to clone the repo.  
    Your trainer will able to help you with this.

3. "Cloning the repo" will create a folder on your computer with the files from this repo.  
Open this folder in Visual Studio Code.

4. Open a command-prompt in this same folder.  
Your trainer can show you how to do this, if you need any help.

5. Run this command to set up the necessary dependencies:  
`poetry install`

6. Run this command to run your code:  
`poetry run start`

7. Run this command to run the tests:  
`poetry run pytest`
(any file named `test_*.py` or `*_test.py` will be discovered and ran automatically)

## Debugging

VSCode debug config has been set up, but you will need to select your virtual environments python interpreter
before running either the tests or app in debug mode. You can do this in VS Code by going to `View`->`Command Palette`,
searching for `Python: Select Interpreter` and then browse your machine to find the appropriate python executable
(e.g. `.venv\Scripts\python.exe` or `.venv\Scripts\python`)

## GUI Dependencies

The application runs a desktop GUI using Tkinter. If you're running an official Python distribution, this will just
work out of the box.

Users relying on third-party Python installations (e.g. Mac/Linux system installs, package managers) may need to configure
Tcl/Tk separately, or download an official Python distribution for use on this codebase.

Mac users can check out <https://www.python.org/download/mac/tcltk/> for further details, or if you're using 
Homebrew you can just run `brew install python-tk`

### Note for WSL users

Sadly, WSL does not support GUIs, so this application will not work from a WSL terminal.
