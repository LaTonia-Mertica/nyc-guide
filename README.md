# <p style="text-align: center">NYC GUIDE</p>

---

#### <p style="text-align: center">*Virtual Tour of The New York City Area from Brooklyn to Staten Island*</p>

<br>

#### **COLLABORATORS**
Kevin Cummings<br>
**Github UN:** [KevinCummings0001](https://github.com/KevinCummings0001)<br>
*'Coding is the language of the future.'*

Jason Doze<br>
**Github UN:** [Jason-Doze](https://github.com/Jason-Doze)<br>
*'Give a man a program, frustrate him for a day. Teach a man a program, frustrate him for a lifetime.'*

La'Tonia Mertica Sheppard Walker<br>
**Github UN:** [LaTonia-Mertica](https://github.com/LaTonia-Mertica)<br>
*'Lean into the challenges of coding.'*

<br>

### **GENERAL SETUP INSTRUCTIONS** 
#### <p style="text-align: left">*we recommend you confirm/test steps outlined below - or elsewhere - before use ... it's for your own code safety*</p>

<br>

**USE VENV TO CREATE & RUN VIRTUAL ENVIRONMENTS:**<br>
1. Execute VENV Command to Create<br>
    1a. Mac aka BASH/ZSH Users run *`python3 -m venv /path/to/new/virtual/environment`*<br>
    1b. PC aka Windows Users run *`c:\>c:\Python35\python -m venv c:\path\to\myenv`*<br>
    **note:** basically you want to run `python3 -m venv django-env` while replacing *django-env* appropriately

2. Execute Activate Command<br>
    2a. MAC aka BASH/ZSH Users run *`source django-env/bin/activate`*<br>
    2b. PC aka Windows Users run *`django-env\Scripts\activate.bat`* and if it doesn't work run *`django-env\Scripts\activate.ps1`*  

3. Execute Run Server Command<br>
    3a. Mac aka BASH/ZSH **and** PC aka Windows Users run *`python`* *`manage.py`* *`runserver`* from app level - which is the same level within the project that contains the `manage.py` file/utility to start Django server (more info below in the run django application instructions)

###### [learn more re: creating and activating virtual environments](https://docs.python.org/3/library/venv.html)

<br>

**USE PIP TO INSTALL PROJECT DEPENDENCIES:**<br>
1. if installing after cloning a repo, run *`pip install -r requirements.txt`* to execute the command to read the requirements file and install everything in it
2. if pip is already installed and want to install a package, run *`pip install insertpackagenamehere`*<br>
    2a. next run *`pip freeze > requirements.txt`*<br>
    2b. this command creates a file called *requirements.txt* while populating the file with dependencies resulting from the install command in step 1 above. from the command line aka terminal run *`cat requirements.txt`* to view dependencies listed in the file 

**note:** pip is the standard package manager for python. [visit python package index to learn more about packages](https://pypi.org/). the command *`pip install`* must be followed by the package you want to install. the command can be run to install the package with or without its dependencies

###### [learn more re: pip install](https://pip.pypa.io/en/stable/cli/pip_install/) 

###### [learn more re: using pip to install project dependencies](https://stackoverflow.com/questions/53925660/installing-python-dependencies-locally-in-project)

<br>

**RUN A DJANGO APPLICATION:**<br>
1. You must use the `manage.py` file/utility to run the server. From the command line/terminal `cd` to the level where the `manage.py` file/utility lives. Run the command *`python`* *`manage.py`* *`runserver`*. You will know the command was successful when you see the following message (or something similar):

"Watching for file changes with StatReloader
Performing system checks...

System check identified no issues (0 silenced).
You have 17 unapplied migration(s). Your project may not work properly until you apply the migrations for app(s): admin, auth, contenttypes, sessions.
Run 'python `manage.py` migrate' to apply them.
May 17, 2019 - 16:09:28
Django version 2.2.1, using settings 'mysite.settings'
Starting development server at `http://127.0.0.1:8000/`
Quit the server with CONTROL-C.
"

**note:** the above message means the django application is running, you must visit the `http://127.0.0.1:8000/` link to access the django application in browser. [the django welcome/homepage](images/django-welcome-homepage.png) may look like an error or exception. this is until you read what it says and follow the instructions to add url endpoints per your project into the browser. for example, `http://127.0.0.1:8000`/(insert your url endpoint here without including the parentheses).

<br>

<img src="images/travel-g580df9aea_1920-courtesy-pixabay.jpg" alt="Virtual Global-Scape" title=" 'Travel' courtesy Pixabay" width="100%"/>
