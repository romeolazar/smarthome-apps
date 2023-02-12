# Home Media Server

LANG=:us:

### Prerequisites.
- A public domain name. Buy one at [https://www.namecheap.com/](https://www.namecheap.com/)
- Use one for free at [https://duckdns.org](https://duckdns.org)
- Docker: [https://docs.docker.com/get-started/](https://docs.docker.com/get-started/)
- Docker Compose: [https://github.com/docker/compose/releases](https://github.com/docker/compose/releases)
- Server platform: [Rocky Linux 8](https://rockylinux.org/download)

# Applications
## smarthome-apps
### [Homebridge](https://homebridge.io)
Homebridge allows you to integrate with smart home devices that do not natively support HomeKit. There are over 2,000 Homebridge plugins supporting thousands of different smart accessories. \
DockerHub: [oznu/homebridge](https://hub.docker.com/r/oznu/homebridge) \
GitHub: [oznu/homebridge](https://github.com/oznu/docker-homebridge)

### [Airconnect]()
Turning Chromecast into Airplay targets. \
DockerHub: [1activegeek/airconnect](https://hub.docker.com/r/1activegeek/airconnect) \
GitHub: [1activegeek/docker-airconnect](https://github.com/1activegeek/docker-airconnect)

## Info
Because all the services are setup with `docker-compose` they can all reach each other by their Docker Compose service name. So for example when connecting Sonarr with Jacket or qBittorrent, then Jackett would be available on `http://jackett/api....`, which makes everything a lot easier.

### Edit the .env file
All configuration to this setup, I've put in the `.env` file, so all you have to do is go through it and edit it to fit your needs.
