# firewall

```sh
firewall-cmd --zone=public --add-port=5000/tcp --permanent
```

## proxychains-ng

```sh
git clone https://github.com/rofl0r/proxychains-ng.git
cd proxychains-ng

./configure --prefix=/usr --sysconfdir=/etc
make
#[optional]
sudo make install
# [optional] installs proxychains.conf
sudo make install-config

# /etc/proxychains.conf
socks5  127.0.0.1 1086
```

## start with proxychains4

```sh
# package.json start cmd
PORT=5000 node .

proxychains4 npm start
```
