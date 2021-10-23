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

## Linux 
- Install Python 3 if you don't already have it (Python 3 ships with pip):
  - Debian based distros: `sudo apt install python3`
  - RedHat based: `sudo dnf install python3` or `sudo yum install python3`
- Install pipenv in the terminal to manage dependencies: `pip3 install pipenv`
- For whichever IDE you're using, install whichever extensions are needed to develop Python applications
- Clone the project to your computer: `git clone https://github.com/NSC-Computer-Science-Club/converger_app.git`
- Move into the project's directory: `cd converger_app`
- Create a virtual environment for the project (that uses Python 3): `pipenv --three`
- Take note of the location of your virtual environment, look for this line in the output:
    - `virtualenv location: /home/jardi/.local/share/virtualenvs/converger_app-UaPtKjcA`
- You can always get the location of your virtual environment by running `pipenv --venv`

Now, it's time to activate your virtual environment. You will install all the dependencies within it.
- Run: `source <path to virtual environment>/bin/activate` (append /bin/activate to your virtual environment's path).

Your prompt will change to `(converger_app) username@hostname` indicating that
you are now working within you virtual environment. We can now install Django.
- Install Django: `pip3 install django`
- Run the server: `python3 manage.py runserver`
- On you browser visit `http://127.0.0.1:8000/` to see your Django ap.
- If you see a warning about unapplied migrations:  `You have unapplied migrations; your app may not work properly until they are applied.`
  - Run 'python manage.py migrate' to apply them. you can ignore them for now.
- Quit the server by either closing the terminal window or pressing `Control + C`.
- To deactivate the virtual environment run: `deactivate`

### Creating an alias for activating your virtual environment

Typing `source /home/jardi/.local/share/virtualenvs/converger_app-UaPtKjcA/bin/activate` every time
I want to work withing that virtual environment gets a little tiring (even with autocomplete).
It might be a good idea to create an alias for it in your `~/.bashrc` file, to append a line
with an alias for that command to your `.bashrc` file do:
  - `echo "alias activate_converger_app='source <path to virtual environment>/bin/activate'" >> ~/.bashrc`
  - Nota bene: Make sure you use two greather than symbols `>>` in that command because using only one will overwrite your .bashrc

The alias will be available the next time you open a bash session (open a terminal). If you want to have it
in your current session you will need to source the .bashrc script: `source ~/.bashrc`

Then:
- To activate the virtual environment run: `activate_converger_app`
- To deactivate the virtual environment run: `deactivate`

## Windows
//TODO


