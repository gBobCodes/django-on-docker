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


NOTES:

DEV
$ docker-compose up --build
is same as
$ docker-compose --file docker-compose.yml --env-file .env up --build

QA
$ docker-compose --file docker-compose-qa.yml --env-file .env.qa --build

PROD
$ docker-compose --file docker-compose-prod.yml --envfile .env.prod --build
