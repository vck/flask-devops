# flask-devops
how to deploy flask web app to gcp + domain [UNFINISHED]

# stack

- flask as web app framework

- virtualenv create new python environment

- nginx as proxy server

- gunicorn as wsgi server

- supervisord as task runner

- gcp as cloud 

# setup

- install all the stack

```
sudo apt install nginx
```

- install pip3/pip 

```
sudo apt install python-pip3
```

- install virtualenv, so we can create new python env 

```
sudo pip3 install virtualenv
```

- create new python env

```
virtualenv env 
```

- activate new env

```
source env/bin/activate
```

- install app related dependencies (don't forget to install flask!)

- install supervisord (use python2.7)

first, we need to install the python2.7 pip

```
sudo apt install python-pip
```

then install supervisord

```
pip install supervisord
```

nuff with the installation part, time to config the proxy server, nginx!

- remove the default nginx config

```
sudo rm /etc/nginx/sites-enabled/default
```

- create new config on `/etc/nginx/sites-enabled/my_awesome_app`
