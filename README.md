# debiantor
Torify Debian
Based on Kalitorify https://github.com/brainfucksec/kalitorify

1. Instructions:

Copy to your /etc/tor/torrc config file:

VirtualAddrNetworkIPv4 10.192.0.0/10
AutomapHostsOnResolve 1
TransPort 9040
SocksPort 9050
DNSPort 5353

2. Run Tor

 service tor start
or
 tor
or
 /etc/init.d/tor start

3. Set permissions and run script as root
chmod +x debiantor.sh
sudo ./debiantor.sh --start

4. Stop script

sudo ./debiantor.sh --stop
