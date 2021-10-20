# Converger App

# Installation
## Mac

- [ ] Download and install Python3 3.8.5
- [ ] Run `pip3 install pipenv` in the terminal to manage dependencies
- [ ] Run `pip3 install django` in the terminal to install Django
- [ ] For whichever IDE you're using, install whichever Python extensions are needed to run Python code
- [ ] Clone project to your computer using `git clone https://github.com/NSC-Computer-Science-Club/converger_app.git`in the terminal
- [ ] Run `pipenv --venv` in the terminal to look for the path to the Python virtual environment on your local computer
  - [ ] If you get an error `pipenv not found` try running `sudo -H pip install -U pipenv`
  - [ ] It should look something like `/Users/kristinjue/.local/share/virtualenvs/converger_app-8tyBun2h`
  - [ ] In VSCode on macOS, find `Select Python Interpreter` by using `Shift-Command-p`
  - [ ] Enter the terminal path and add to the end `/bin/activate`, so it looks something like `/Users/kristinjue/.local/share/virtualenvs/converger_app-8tyBun2h/bin/activate`
  - [ ] In the .vscode folder, replace `/Users/kristinjue/.local/share/virtualenvs/converger_app-8tyBun2h/bin/activate` with the path to the virtual environment on your local machine.
- [ ] Run `python3 manage.py runserver`
- [ ] Django web app should open at location `http://127.0.0.1:8000/`
- [ ] If you see a warning about unapplied migrations, like  `You have unapplied migrations; your app may not work properly until they are applied.
Run 'python manage.py migrate' to apply them.` you can ignore them for now.
- [ ] Quit the server by either closing the terminal window or running `Control C` on macOS

## Windows
//TODO

## Linux 
//TODO


