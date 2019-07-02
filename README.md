[![Django](https://img.shields.io/badge/Django-2.2.3-green.svg)](https://www.djangoproject.com/weblog/2019/jul/01/security-releases/)
[![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](LICENSE)

# How To Install Django In Mac
src: https://appdividend.com/2018/03/28/how-to-install-django-in-mac/#Step_1_Install_Python_on_Mac


### Set up virtualenv
```
virtualenv ~/virtualenv
```


### Launch virtualenv
```
source ~/virtualenv/bin/activate
```

### Requirements
src: https://gist.github.com/Siltaar/9441a525d3a580311035fa2f3f431baa

[`requirements.txt`](requirements.txt) file installs all the necessary `modules` for your project:


```
cd ~/virtualenv
sudo pip3 install -r ~/virtualenv/requirements.txt
```


### Launch Django project
```
cd ~/virtualenv/rioanalytics
python3 ~/virtualenv/rioanalytics/manage.py runserver
```


### Creating an admin user
src: https://docs.djangoproject.com/en/2.2/intro/tutorial02/
```
cd ~/virtualenv/rioanalytics
python3 ~/virtualenv/rioanalytics/manage.py createsuperuser
Username:
Email address:
Password:
```


### Extract Sqlite Database
src: https://stackoverflow.com/questions/3034910/whats-the-best-way-to-migrate-a-django-db-from-sqlite-to-mysql
```
cd ~/virtualenv/rioanalytics
python3 ~/virtualenv/rioanalytics/manage.py dumpdata > ~/virtualenv/rioanalytics/datadump.json
```


###### References:
- [Mastering GitHub Markdown](https://guides.github.com/features/mastering-markdown/)
- [Markdown Tutorial](https://github.com/luong-komorebi/Markdown-Tutorial/blob/master/README_fr.md)
