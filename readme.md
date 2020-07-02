1. The folder -- RNA is the name of the whole website, the files in the folder were generated automatically.
    * __init__.py       indicates this folder is for python
    * settings.py       sets some info about the website
    * urls.py           contains all urls in the website (kind of map)
    * wsgi.py           WSGI config for rna project.

2. The folder -- analysis (The application in the website)
    * APD.py            python file for RNA-Aptamer analysis
    * forms.py          check the formats of submitted forms
    * models.py         used to manage database
    * views.py          process the information submitted from the user

    The following files are generated automatically:
        * migrations       used to manage database
        * __init__.py      indicates this folder is for python
        * admin.py
        * apps.py          show all the apps in the website

3. The folder -- download (The place to store the files such as APD.zip which can be downloaded from the website by users directly)

4. The folder -- templates
    * index.html           sets up the appearance of the website


manage.py  it's an important file to manage the whole project. We can run the server by command line: python manage.py runserver

All files above are important, we can delete the rest. Meanwhile, the three files: forms.py, views.py , index.html are modified frequently
which means we can modify them to satisfy our different needs.

