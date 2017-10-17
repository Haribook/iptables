# iptables
Forward all the packets on port 80 to the internal port 8080
iptables -A PREROUTING -t nat -i eth0 -p tcp --dport 80 -j REDIRECT --to-port 8080

save iptables with below command
apt-get install iptables-persistent –y
