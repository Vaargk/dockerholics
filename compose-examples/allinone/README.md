# DL - download pipeline stack
This will install and create containers for the following apps
- Plex
- Posterr
- Watchtower
- Dozzle
- Autoheal
- Radarr
- Sonarr
- Lidarr
- Readarr
- Prowlarr
- Bazarr
- Sabnzbd
- Qbittorrent
> Do not use Qbittorrent until it is protected by a VPN

## Prerequisites
This will install as-is, however best with OpenVPN/Wireguard/Another VPN?

### Folders
The following folders should be created
- docker
> - /c/docker (on windows)
> - ~/docker (on linux)
> - /volume1/docker (on Synology)
- *somewhere*/downloads
- *somewhere*/incomplete
> These above folders are for partial and completed downloads. Put them under a folder wherever you wish.
- {docker}/prowlarr
- {docker}/sonarr
- {docker}/radarr
- {docker}/lidarr
- {docker}/bazarr
- {docker}/readarr
- {docker}/sabnzbd
- {docker}/plex
- {docker}/plex/transcode
- {docker}/plex/config
- {docker}/portainer
- {docker}/tautulli
- {docker}/posterr
- {docker}/poster/config
- {docker}/poster/randomthemes
- {docker}/gaps
> The above folders should be under your `docker` folder.

Your media path should be one top-level folder with sub folders for different media types 
> For example:
> - media
>   - movies
>   - tv
>   - music
>   - ebooks

### Changes to .env file
Review the .env and update
- TZ
- PUID
- PGID
- Path values
- plex-specific values
