# Installation

## Download

Execute the following command.
```
mkdir work
cd work
wget https://github.com/omotenashicoin-project/OmotenashiCoin-HDwalletbinaries/raw/master/stable/backend-mtns_1.7.3-satoshilabs-1_amd64.deb
wget https://github.com/omotenashicoin-project/OmotenashiCoin-HDwalletbinaries/raw/master/stable/blockbook-mtns_0.3.1_amd64.deb
```

## Installation
Execute the following command.
```
sudo apt install ./backend-mtns_1.7.3-satoshilabs-1_amd64.deb
sudo apt install ./blockbook-mtns_0.3.1_amd64.deb
service backend-mtns start
service blockbook-mtns start

```

## Access from your browser
Start your browser.
Enter the following URL.

ex)
```
https://yourdomain_or_globalIPaddress:9194
```

### FAQ
#### Check the service startup status
```
ps axu | grep mtns
```
ex)Normal startup logs
```
mtns      1006 85.1  0.2 1425344 36364 ?       SLsl 16:02  94:04 /opt/coins/nodes/omotenashicoin/bin/omotenashicoind -datadir=/opt/coins/data/omotenashicoin/backend -conf=/opt/coins/nodes/omotenashicoin/omotenashicoin.conf -pid=/run/omotenashicoin/omotenashicoin.pid
mtns      1042  0.9  1.6 1711296 205436 ?      SLsl 16:02   1:00 /opt/coins/nodes/omotenashicoin/bin/omotenashicoind -datadir=/opt/coins/data/omotenashicoin/backend -conf=/opt/coins/nodes/omotenashicoin/omotenashicoin.conf -pid=/run/omotenashicoin/omotenashicoin.pid
ubuntu   12589  0.0  0.0  22556  1104 pts/2    S+   17:53   0:00 grep --color=auto mtns
```

#### Check the service start result
```
systemctl status backend-mtns
```
or
```
systemctl status blockbook-mtns
```
ex) Normal startup
```
● backend-mtns.service - Omotenashicoin backend daemon
   Loaded: loaded (/lib/systemd/system/backend-mtns.service; enabled; vendor preset: enabled)
   Active: active (running) since Thu 2020-01-23 16:02:42 JST; 1h 52min ago
  Process: 900 ExecStart=/opt/coins/nodes/omotenashicoin/bin/omotenashicoind -datadir=/opt/coins/data/omotenashicoin/backend -conf=/opt/coins/nodes/omotenashicoin/omotenashicoin.conf -pid=/run/omotenashico
 Main PID: 1006 (omotenashicoind)
    Tasks: 21 (limit: 4915)
   CGroup: /system.slice/backend-mtns.service
           mq1006 /opt/coins/nodes/omotenashicoin/bin/omotenashicoind -datadir=/opt/coins/data/omotenashicoin/backend -conf=/opt/coins/nodes/omotenashicoin/omotenashicoin.conf -pid=/run/omotenashicoin_test

 yourhostname systemd[1]: Starting Omotenashicoin backend daemon...
 yourhostname systemd[1]: backend-mtns.service: Can't open PID file /run/omotenashicoin/omotenashicoin.pid (yet?) after start: No such file or directory
 yourhostname systemd[1]: Started Omotenashicoin backend daemon.
```

#### When backend (when OmotenashiCoind does not start) does not start
```
rm -rf /opt/coins/data/omotenashicoin/backend/
service backend-mtns start
```

#### Delete installation program
```
service blockbook-mtns stop
service backend-mtns stop
rm -rf /opt/coins/data/omotenashicoin
rm -rf /opt/coins/blockbook/omotenashicoin
apt remove --purge blockbook-mtns
apt remove --purge backend-mtns
```



