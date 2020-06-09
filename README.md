# maroph.github.io/openhpi-git
GitHub Projekt für den OpenHPI Git Kurs

---

### Install missing Python3 software
If pip for Python3 and/or the Python3 venv module aren't installed on your system
use the following commands as administrator (root):

    sudo apt install python3-pip
    sudo apt install python3-venv

### How the virtual environment is created
The following commands are used to build the needed virtual environment:

    python3 -m venv ./venv
    source ./venv/bin/activate
    python -m pip install --upgrade pip
    python -m pip install --upgrade setuptools
    python -m pip install --upgrade wheel
    python -m pip install --requirement ./requirements.txt

##  Build the docs

    source venv/bin/activate
    mkdocs build


##  Push to GitHub

    git commit -m "my commit message"
    git push

