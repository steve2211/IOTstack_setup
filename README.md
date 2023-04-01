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
   * *influxdb2*
   * *mosquitto*
   * *nodered*
	   &rarr; *Select & overwrite addons list*
   * *portainer ce*
10.  *Docker Commands &rarr; Start stack*
