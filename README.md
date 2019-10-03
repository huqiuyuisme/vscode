wget --no-check-certificate https://raw.githubusercontent.com/teddysun/shadowsocks_install/master/shadowsocksR.sh

chmod +x shadowsocksR.sh

./shadowsocksR.sh 2>&1 | tee shadowsocksR.log

wget --no-check-certificate https://raw.githubusercontent.com/teddysun/across/master/bbr.sh 

chmod +x bbr.sh && ./bbr.sh

Ubuntu/Debian

#!/bin/sh   
apt-get update
apt-get install git python-m2crypto libsodium18
cd /usr/local
git clone -b manyuser https://github.com/shadowsocksrr/shadowsocksr.git
cd shadowsocksr
bash initcfg.sh

CenOS—-待验证可用性

#!/bin/sh
yum update
yum install git python-m2crypto libsodium18
cd /usr/local
git clone -b manyuser https://github.com/shadowsocksrr/shadowsocksr.git
cd shadowsocksr
bash initcfg.sh


cd /usr/local/shadowsocksr

vim user-config.json

cd /usr/local/shadowsocksr/shadowsocks

bash ./logrun.sh

bash ./tail.sh

bash ./stop.sh

bash ./logrun.sh

wget --no-check-certificate https://github.com/Ellean/across/raw/master/bbr.sh && chmod +x bbr.sh && ./bbr.sh
