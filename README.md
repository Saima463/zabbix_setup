# How to Install Zabbix

```
wget https://repo.zabbix.com/zabbix/4.0/ubuntu/pool/main/z/zabbix-release/zabbix-release_4.0-3+xenial_all.deb

sudo dpkg -i zabbix-release_4.0-3+xenial_all.deb

apt-get install zabbix-agent 

```

## Configure zabbix_agentd.conf 

 nano /etc/zabbix/zabbix_agentd.conf 

Add the following lines,

```
Server=5.9.238.114

ServerActive=127.0.0.1

```

## Check Service Status

```
systemctl status zabbix-agent

systemctl enable zabbix-agent
```

