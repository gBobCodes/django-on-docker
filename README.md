# django-on-docker

## Starting Development

Download the source
```
$ git clone git@github.com:gBobCodes/django-on-docker.git
$ cd django-on-docker
```

Build Docker Images
```
$ docker-compose up -d --build
```

Acces the python container
```
$ docker-compose exec api /bin/bash
```

Edit the source code on your local device, not in the python container.
