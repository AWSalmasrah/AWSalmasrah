# Run your First EC2

## Step 1 — Update and upgrade

Before we do anything else, let’s make sure we update the local package index and upgrade the system. This makes sure everything is up to date and prevents any errors due to deprecations.

```
$ sudo apt-get update
$ sudo apt-get -y upgrade
```
## Step 2 — Set up Python 3

Check the Python version installed in the system, as of this article Python 2 is officially deprecated so you should be using Python 3 on new projects. Ubuntu 20.04 comes with Python 3 pre-installed.

```
$ python3 -V
```
You should get an output similar to this.
```
Python 3.8.5
```
Install PIP to manage software packages for Python.
```
$ sudo apt install -y python3-pip
```
Check that pip3 installation was successful.
```
pip3 -V
```
Output
```
pip 20.0.2 from /usr/lib/python3/dist-packages/pip (python 3.8)
```
Install other required dependencies to make sure you have a robust development environment.
```
$ sudo pip install flask
```
## Step 3 — Version Control

For this tutorial, you will be using GIT to clone our project into this server. Version control allows for easier codebase management and team collaboration. Ubuntu 20.04 also comes with GIT pre-installed.
```
$ git --version
```
```
git version 2.25.1
```

## Step 4 — Clone the Repo

```
git clone https://github.com/AWSalmasrah/AWSalmasrah.git
```
## Step 5 — Run the Flask application
```
cd E3 - Run your First EC2
python3 app.py
```
```

