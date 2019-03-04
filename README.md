# aloe-selenium-python
# Python 3.7 Installation + Selenium + Aloe - Walk Through
***
### WHAT YOU NEED
Homebrew, Python3, Selenium and Aloe.

#### *Some Facts:*
* Python 3 is not pre-installed by default on MacOS.
* As a recommendation, use homebrew package manager for MacOS.
* If the Homebrew version of Python 2 is installed then pip2 will point to Python 2. If the Homebrew version of Python 3 is installed then pip will point to Python 3.

### Install Homebrew
Access https://brew.sh/
Run this command on the terminal:

### IMAGE -------

To verify that it was installed correctly, please type the following in your terminal:

```
brew --version
```

### Install python 3.7.x

```
brew install python3
```
To verify that it was installed correctly, please type the following in your terminal:

```
python3 --version
```
We also need to confirm that we have PIP (package management system) installed after installing Python.

Confirm the PIP version:

```
pip3 --version
```

### IMAGE -------

### Install virtualenv

Virtualenv is a tool to create isolated Python environments. It creates an environment that has its own installation directories.

```
pip3 install virtualenv
```

### IMAGE -------

**This action could throw an error related to denied permissions in a specific folder, to fix it, add --user at the end of the command:*

```
pip3 install virtualenv --user
```

When you have multiple environments with different packages, you can activate or deactivate each one of them in order to work with the one you need at the moment.

### Create a virtualenv:

```
virtualenv env --python=python3
```

### Activate the virtualenv:

```
source <desired-path>/bin/activate
```

### Deactivate the virtualenv:
```
deactivate
```

You can use the command ```pip freeze``` to see all installed software within a virtual environment.


### Selenium Webdriver

Supports:

* Google Chrome
* Internet Explorer 7, 8, 9, 10, and 11 on appropriate combinations of Vista, Windows 7, Windows 8, and Windows 8.1. As of April 15 2014, IE 6 is no longer supported. The driver supports running 32-bit and 64-bit versions of the browser where applicable
* Firefox: latest ESR, previous ESR, current release, one previous release
* Safari
* Opera
* HtmlUnit
* phantomJS
* Android (with Selendroid or appium)
* iOS (with ios-driver or appium)

Selenium can be customized, and it is Open Source, so it means the source code can always be downloaded and modified.

### Install Selenium
```
pip3 install selenium
```

### IMAGE ----

Selenium requires a driver to interface with the chosen browser.
Put the desire webdriver in your path:
Chrome: http://chromedriver.chromium.org/downloads
Firefox: https://github.com/mozilla/geckodriver/
Others: https://www.seleniumhq.org/download/

### Install Aloe webdriver

```
pip3 install aloe
```
**It could throw an error related to denied permissions in a specific folder:*

### IMAGE ----

To fix that error, just add ```--user``` to ```pip3 install aloe```

So:

```pip3 install aloe --user```

### IMAGE ----

That's all you have to do to install and configure Python, virtualenv, selenium and aloe on OSX.


