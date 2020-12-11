# Android application: Calculator

Kivy is a framework for building mobile applications in Python. This repository illustrates some of the basic aspects of app development such as events, labels and layouts. Finally, a simple calculator is produced in Kivy and complied to work for android.

Note that Kivy works for Python 3.6 and prior versions. 


# Requirments
__Recommended__: Create a virtual environment. (Ubuntu description)
#### Step 1: Update your repositories
```console
user@user_name:~$ sudo apt-get update

```
#### Step 2: Install pip for Python 3
```console
user@user_name:~$ sudo apt-get install build-essential libssl-dev libffi-dev python-dev
```
```console
user@user_name:~$ sudo apt install python3-pip
```
#### Step 3: Use pip to install virtualenv
```console
user@user_name:~$ sudo pip3 install virtualenv
```
#### Step 4: Launch your Python 3 virtual environment, here the name of my virtual environment will be _kivy_project_.
__Note__: For Python2 use __virtualenv__ and Python3 use __venv__
```console
user@user_name:~$ venv -p python3 kivy_project
```
#### Step 5: Activate your new Python 3 environment. There are two ways to do this
```console
user@user_name:~$ .kivy_project/bin/activate 
```
or
```console
user@user_name:~$ source kivy_project/bin/activate 
```
(which does the same thing).
You can make sure you are now working with Python 3
```console
user@user_name:~$ python3 --version 
```
### Requirements
The soft dependencies are:
```console
user@user_name:~$
sudo apt-get install -y \
    libsdl2-dev \
    libsdl2-image-dev \
    libsdl2-mixer-dev \
    libsdl2-ttf-dev \
    libportmidi-dev \
    libswscale-dev \
    libavformat-dev \
    libavcodec-dev \
    zlib1g-dev
```
Install gstreamer for audio, video (optional)
```console
user@user_name:~$
sudo apt-get install -y \
    libgstreamer1.0 \
    gstreamer1.0-plugins-base \
    gstreamer1.0-plugins-good
```
Installing Kivy: 
```console
user@user_name:~$
python3 -m pip install kivy[base]
```
__Note__: Downloads _base_ version, change to _full_ for extended Kivy library; audo, visual etc.

# Files:
- __requirements.txt__: use ```console user@user_name:~$ pip3 install -r requirements.txt ```
- kivy_calculator.py: Main demonstrative calculator application
- kivy_displaying_image.py: How to display an image
- kivy_events.py: Event handling with Kivy
- kivy_Hello_Kivy.py: _Hello_ _World!_
- kivy_KV_language.py: KV language; separating logic from aesthetics
- kivy_project: Virtual environment
- kivy_UI_layout.py: Kivy aesthetics
- app: Folder containing _'main.py'_(same as kivy_calculator.py, but renamed) and _buildozer.spec_ file 
- buildozer: Package for compiling applications 
