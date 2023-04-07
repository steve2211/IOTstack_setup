# IOTstack_setup

1. `sudo apt update -y && sudo apt full-upgrade -y && sudo apt autoremove -y`
2. `curl -fsSL https://raw.githubusercontent.com/SensorsIot/IOTstack/master/install.sh | bash`
3. `sudo groupadd docker`
4. `sudo usermod -aG docker $USER`
5. `sudo reboot`
6. `cd IOTstack`
7. `./menu.sh`
8. *Build Stack*
9. * *grafana*
   * *homebridge*
   * *influxdb*
   * *mosquitto*
   * *nodered*
	   &rarr; *Select & overwrite addons list*
   * *portainer ce*
10.  `nano services/nodered/Dockerfile`
* `RUN apk add --no-cache sudo curl build-base g++ libpng libpng-dev jpeg-dev pango-dev cairo-dev giflib-dev python3`
* `RUN apk --no-cache add ca-certificates wget && wget -q -O /etc/apk/keys/sgerrand.rsa.pub https://alpine-pkgs.sgerrand.com/sgerrand.rsa.pub && wget https://github.com/sgerrand/alpine-pkg-glibc/releases/download/2.29-r0/glibc-2.29-r0.apk && apk add glibc-2.29-r0.apk && npm install canvas`
11.  *Docker Commands &rarr; Start stack*
12. `docker exec mosquitto mosquitto_passwd -b /mosquitto/pwfile/pwfile public public`
