# Docker Compose for Raspberry Pi

The docker-compose.yml file is configured for Raspberry Pi 4 (especially but not limited) and has 4 containers:
- mysql, based on [biarms/mysql:5.5](https://hub.docker.com/r/biarms/mysql)
- zabbix server, based on [zabbix/zabbix-server-mysql:alpine-5.2.5](https://hub.docker.com/r/zabbix/zabbix-server-mysql)
- zabbix frontend, based on [zabbix/zabbix-web-apache-mysql:alpine-5.2.5](https://hub.docker.com/r/zabbix/zabbix-web-apache-mysql)
- zabbix-agent, based on [zabbix/zabbix-agent2:alpine-5.2.5](https://hub.docker.com/r/zabbix/zabbix-agent2)

Zabbix DB is configured for **Cyrillic** and **Latin**.

Please replace **YOUR-PASSWORD** with your strong password :-)

## Run
Just run the following command in the folder where the docker-compose.yml file is located:

<code>docker-compose up -d</code>

After that you can reach web interface on port 8080:
http://your-raspberry-ip:8080
