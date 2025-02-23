# Repo local Pypi comme cache d'un repo distant

devpi registry :
- https://devpi.net/docs/devpi/devpi/stable/+d/quickstart-pypimirror.html
- https://github.com/muccg/docker-devpi
- https://hub.docker.com/u/muccg


## Configuration pour utiliser ce repo :
Completer le fichier `pip.ini` ou `pip.conf` avec :
```ini
[global]
index-url = http://monuser:monpassword@localhost:3141/monuser/monindex/simple/
trusted-host = localhost
```

## Mettre a jour les requirements
- uv pip compile requirements.in -p 3.12 -o requirements.txt

## Configuration des users sur devpi
...

## Verification des packages en cache
- ls root/.devpi/server/
