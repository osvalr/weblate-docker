# weblate-docker

[![Build Status](https://travis-ci.org/nijel/weblate-docker.svg?branch=master)](https://travis-ci.org/nijel/weblate-docker)

## Docker container for Weblate

Documentation is available in Weblate documentation:

https://docs.weblate.org/en/latest/admin/deployments.html#docker

## Steps to get Weblate up and running Weblate:

### Clone repo

```bash
$ git clone git@github.com:osvalr/weblate-docker.git
```

### Get into folder and run the following commands (taken from travis conf file)

```bash
$ cd weblate-docker
$ docker-compose build
$ docker-compose run weblate migrate --noinput
$ docker-compose run weblate collectstatic --noinput
$ docker-compose run weblate createadmin
```
## IMPORTANT: Copy the password to clipboard that it shows after last command gets executed

##. Get running weblate

```bash
$ docker-compose up
```

### Open web-browser with http://localhost:8000
