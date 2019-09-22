wget --no-check-certificate https://raw.githubusercontent.com/teddysun/shadowsocks_install/master/shadowsocksR.sh

chmod +x shadowsocksR.sh
./shadowsocksR.sh 2>&1 | tee shadowsocksR.log
wget --no-check-certificate https://raw.githubusercontent.com/teddysun/across/master/bbr.sh && chmod +x bbr.sh && ./bbr.sh
