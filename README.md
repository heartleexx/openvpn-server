# Steps
## 1. Download openvpn-install.sh
```
wget https://raw.githubusercontent.com/heartleexx/openvpn-server/refs/heads/main/openvpn-install.sh -O openvpn-install.sh
```
or
```
curl -L https://raw.githubusercontent.com/heartleexx/openvpn-server/refs/heads/main/openvpn-install.sh -o openvpn-install.sh
```

## 2. Run openvpn-install.sh to install vpn server and create first client.
```
sudo bash ./openvpn-install.sh
```

After that run the same command to create new clients
```
sudo bash ./openvpn-install.sh
```

## 3. If needed to change openvpn server config
```
vim /etc/openvpn/server/server.conf
```
and then restart openvpn serverK
```
sudo systemctl restart openvpn-server@server.service
```
