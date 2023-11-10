# BeeWare App Test

## Test for Python-based BeeWare App

Using the [BeeWare](https://beeware.org) Tutorial ([link here](https://docs.beeware.org/en/latest/tutorial/tutorial-0.html)) to test features of [Briefcase](https://briefcase.readthedocs.io/en/stable/) (converts Python code to standalone native apps) and [Toga](https://toga.readthedocs.io/en/stable/) (Pythong native/OS native, class-platform GUI toolkit)

## Common commands for BeeWare 

See [tutorial](https://docs.beeware.org/en/latest/tutorial/tutorial-0.html).

Create and use virtual environment:
```
% python -m venv venv
% source venv/bin/activate
```
Install briefcase
```
(venv) $ python -m pip install briefcase
```
Creating application scaffold:
```
(venv) $ briefcase create
```
For building application scaffold:
```
(venv) $ briefcase build
```
For building installer (```--adhoc-sign``` is for local use only, not for wide deployment):
```
(venv) $ briefcase package --adhoc-sign 
```
For updating the app, after updating any code, run the following:
```
(venv) $ briefcase update
```
For updating, building, and running the app in a single command:
```
(venv) $ briefcase run -u
```
***for iOS***

Building an iOS app
```
(venv) $ briefcase create iOS
```
Running an iOS app
```
(venv) $ briefcase run iOS
```