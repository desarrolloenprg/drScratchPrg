drScratch
=========

drScratch is an analytical tool that evaluates your Scratch projects in a variety of computational areas to provide feedback on aspects such as abstraction, logical thinking, synchronization, parallelization, flow control, user interactivity and data representation. This analyzer is a helpful tool to evaluate your own projects, or those of your Scratch students.

You can try a beta version of drScratch at http://drscratch.org

------------------------------------

## Dependencies
 - Python 2.7.14
 - Django 1.7 python frameWork
 - kurt python module
 - hairball python module
 - gspread python module
 - oauth2client python module

------------------------------------

## ASSEMBLE THE PROJECT

>  1.- Install Git ( https://git-scm.com )
>
>  2.- Install Python 2.7.14 
>
>  3.- [(2)STEPS] Follow steps [ Pip install - Python 2.7 - Windows 7/10 ] 
>
>  4.- cd (choose or make a folder) and copy the project
>
>  5.- [(4)STEPS]Follow steps [ Requirements ]  
>
>  6.- [(5)STEPS] Follow steps [ yolk (for check the requirements) ] 
>
>  7.- [(6)STEPS] Follow steps [ Django (django configuration) ] 
>
>  8.- drScratch.exe - (run local server) 

+====================================================

###### + [(2)STEPS] ======= Pip install/Python 2.7
```
URL : http://www.aaronstannard.com/how-to-setup-a-proper-python-environment-on-windows/
1.- add path to environment variables
2.- path = "C:\Python27\Scripts;C:\Python27"
```

###### + [(4)STEPS] ======= Requirements
```
$ cd drScratch (go to the root folder of the project)
$ pip install -r requirements.txt
```

###### + [(5)STEPS] ======= yolk (for check the requirements)
```
URL: https://pypi.python.org/pypi/yolk/0.4.3
$ yolk -l
```

###### + [(6)STEPS] ======= Django
```
URL : https://docs.djangoproject.com/en/1.7/
URL TUTORIAL : https://docs.djangoproject.com/en/1.7/intro/tutorial01/
$ python manage.py makemigrations app
$ python manage.py sqlmigrate app 0001
$ python manage.py migrate
$ python manage.py runserver
```

------------------------------------

## EXTRA INFORMATION 

##### kurt
```
https://pypi.python.org/pypi/kurt
Library for reading/writing MIT's Scratch file format.
Kurt is a Python library for working with Scratch project files.
pip install kurt
```

##### hairball
```
URL : https://pypi.python.org/pypi/hairball/0.3
URL : https://github.com/ucsb-cs-education/hairball

Hairball is a plugin-able framework useful for 
static analysis of Scratch projects.

$ pip install hairball

Once you installed the original hairball distribution
you should replace its files with the ones in our
fork
URL: https://github.com/jemole/hairball
```

##### gspread oauth2client ( Python Lib )
```
URL : https://github.com/burnash/gspread
URL TUTORIAL : https://github.com/burnash/gspread
$ pip install gspread oauth2client 
```

##### Google Drive and Google Sheets API
```
URL : https://console.developers.google.com
URL TUTORIAL : 
Login
habilitar Google Drive API
habilitar Google Sheets API
Credenciales / CREAR miembro (cuentas de servicios)
```

##### Compilando .exe para hacerlo modo escritorio
```
Requiere Visual Studio Compiler C++ 
URL : https://msdn.microsoft.com/en-us/library/9s7c9wdw.aspx
$ cl /EHcs main.cpp 
or
$ cl /EHcs main.cpp /Fe:drScratch
```