# Docker compose setup

Requires:
* .env
* docker-compose 

## To run

`docker-compose up`

## .env

* USERNAME
* PASS
* DOCKER\_UID
  * need to match volume write permissions
* DOCKER\_GID
  * need to match volume write permissions
* CONFIG
  * needed for running containers multiple times
* RADARR\_VOLUME
  * base folder for radarr, sonarr, transmission

## Setup

* linuxserver.io images
  * (radarr)[https://docs.linuxserver.io/images/docker-radarr]
  * (sonarr)[https://docs.linuxserver.io/images/docker-sonarr]
  * (transmission)[https://docs.linuxserver.io/images/docker-transmission]
    * can be swapped with other torrent
  * (jellyfin)[https://docs.linuxserver.io/images/docker-jellyfin]
    * can swap for plex, etc
  * (prowlarr)[https://github.com/linuxserver/docker-prowlarr]
    * only develop and nightly tags
    * requires some initial configuration to connect with sonarr
      * index
      * client

Pretty confusing to setup first time. Conflicting documentation between linuxserver
and (servarr)[https://wiki.servarr.com/radarr] basically jumped around both to get
setup. When radarr & sonarr running still need to add /movies, /tv, and /downloads
for them to work correctly.
