# mqtt-telegraf-influxdb-grafana
Docker compose repo with MQTT, Telegraf, InfluxDB and Grafana.

Full set-up from scratch :

- sudo apt update
- sudo apt upgrade

- login SSH as root (default SSH port 22 is on)
- add a other user with root rights :
sudo useradd -ou 0 -g 0 arjan
sudo passwd arjan
usermod -aG sudo arjan
chsh -s /bin/bash arjan
- generate SSH keys with putty gen (save private and public key)
- make folder and key file MAKE SURE YOUR ARE LOGGED IN AS ARJAN
mkdir ~/.ssh
chmod 700 ~/.ssh
nano ~/.ssh/authorized_keys
- past public key and save
chmod 600 ~/.ssh/authorized_keys
- change ssh config
sudo nano /etc/ssh/sshd_config
- change port to 2211 and passwordauthentication to no and reboot


