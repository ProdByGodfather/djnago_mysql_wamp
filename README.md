# djnago_mysql_wamp
Connecting to mysql database in wampserver using Django.
<br>
first you need go to `requirements.txt` and install this libraries, for install with cmd:
```
pip install -r requirements.txt
```

On `django_mysql/settings.py` I write default Connection on Wampserver mysql with django (on default user):
```
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.mysql',
        'NAME': 'mahdi', # db Name
        'USER': 'root', # db Username
        'PASSWORD': '', # db Password
        'HOST':'localhost', # db host
        'PORT':'3306', # db port, on wampserver default port is 3306
    }
}
```
now you can migrate to mysql wampserver with this command:
```
python manage.py migrate
```

