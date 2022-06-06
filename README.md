# Wireshark installation
In order to install **Wireshark** on a Debian based operating system run the following commands on the terminal:
```sh
sudo apt-get update && sudo apt-get upgrade -y
```
```sh
sudo apt-get install wireshark
```
```sh
sudo groupadd wireshark
```
```sh
sudo usermod -a -G wireshark pi
```
```sh
sudo chgrp wireshark /usr/bin/dumpcap
```
```sh
sudo chmod 750 /usr/bin/dumpcap
```
```sh
ls -al /usr/bin/dumpcap
```
```sh
sudo setcap cap_net_raw,cap_net_admin=eip /usr/bin/dumpcap
```
```sh
sudo getcap /usr/bin/dumpcap
```
```sh
wireshark
```

