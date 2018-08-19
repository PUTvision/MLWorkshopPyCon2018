# Say hello to machine learning in Python @ PyConPL 2018
If you encounter any issues when following these instructions or want to know some additional rationale behind specific
steps - **don't hesitate to ask us questions**.

## Installing Python
The workshop uses Python 3. We recommend using up-to-date version (Python 3.7), but previous ones should also work fine.

### Linux
There is a high chance that you have Python 3 already installed. You can check that by running the following command in
your terminal:
```
python3 --version
```

#### Debian / Ubuntu / Mint
```
sudo apt install python3
```
#### Fedora
```
sudo dnf install python3
```
#### Other
If you use less common distribution you probably know how to acquire Python 3.

### Windows
You can download and use current Python 3 installer from [https://www.python.org/downloads/windows/]().

Although you probably won't encounter any problems with 32-bit (x86) version we recommend using 64-bit (x86-64) release
on 64-bit system (you almost certainly have it) as it will be able to allocate more memory and therefore will allow you
to work with more data at the same time.

### MacOS
We will use Python 3 from Homebrew package manager.
#### Setup Homebrew
Install Xcode as Homebrew depends on it:
```
xcode-select --install
```

Install Homebrew:
```
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

#### Install Python 3
```
brew install python3
```

## Installing and running Jupyter Notebook
### Setup virtualenv for the workshop
This will allow to install packages locally instead of system-wide. You can have many virtualenvs that include project
specific versions of libraries.

You can create virtualenv in the directory that already contains workshop files using command line:
```
cd /path/to/MLWorkshopPyCon2018
python3 -m venv workshop_venv
```

To activate virtualenv and start installing packages inside it use:
```
source workshop_venv/bin/activate
```

### Install Jupyter Notebook
You can install Jupyter Notebook inside virtualenv using Python package manager (*pip*). Jupyter documentation also
recommends upgrading *pip* to the latest version so we will perform both of those operations:
```
pip3 install --upgrade pip
pip3 install jupyter 
```

### Run Jupyter Notebook server
You can run Jupyter Notebook server from the command line:
```
jupyter notebook
```

This command should start a server and open your default web browser. If it didn't or if you prefer to use other browser
you can navigate to [http://localhost:8888/](). 

The console window can be minimized, but don't close it as we need Jupyter server to keep running.

### Open workshop notebook
After opening the notebook app in your web browser you will see a list of files located in the directory you ran the
server from.

You can click on `Say hello to machine learning in Python.ipynb` file to open the workshop notebook.  

## Fallback solution
If you had some serious problems with following the steps or you simply don't want to install anything on your computer
you can use [Google Colaboratory](https://colab.research.google.com) for this workshop.
