# Installation du projet

Présentation général du projet : 

//TODO 
.... 

## Récupérer le projet 

```
git clone TODO
```

## Lancer docker

créer le fichier .env.local à la racine du projet

Modifier les port dans le .env.local.env en fonction des autres images docker
- PHP_EXT_PORT_1
- PHP_EXT_PORT_2
- BDD_EXT_PORT


lancer Docker pour la première fois : 
```
docker compose --env-file .env.local up --build --force-recreate -d
```

pour debuguer le build 
```
docker-compose build --no-cache 2>&1 | tee build_logs.txt
``` 