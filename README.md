[![Build Status](https://travis-ci.org/rileyschuit/rpi-docker-sickrage.svg?branch=master)](https://travis-ci.org/rileyschuit/rpi-docker-sickrage)

# Docker sickrage to run on a Raspberry Pi   
This is a Dockerfile to set up "SickRage" - (https://sickrage.github.io/)  
### Build from docker file  
```
git clone git@github.com:rileyschuit/rpi-docker-sickrage.git
cd docker-sickrage
docker build -t rpi-docker-sickrage .
```
  
### Pull from docker hub:    
```
docker run --restart=always -d -h *your_host_name* -v /*your_config_location*:/config  -v /*your_videos_location*:/data -p 8081:8081 sickrage
```

