# Docker compose setup

Requires:
* .env
* docker-compose 

## To run

`docker-compose up`

## .env

* USERNAME
* PASS
* PEERFLIX\_VOLUME
  * only need this setup if want to persist data
* DOCKER\_UID
  * need to match volume write permissions
* DOCKER\_GID
  * need to match volume write permissions
* CONFIG
  * needed for running containers multiple times
* RADARR_VOLUME
  * base folder for radarr, sonarr, transmission
