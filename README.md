# Docker Compose for Raspberry Pi

The docker-compose.yml file is configured for Raspberry Pi 4 and has 3 containers:
- mysql, based on [biarms/mysql:5.5](https://hub.docker.com/r/biarms/mysql)
- zabbix server, based on [zabbix/zabbix-server-mysql:alpine-5.2.5](https://hub.docker.com/r/zabbix/zabbix-server-mysql)
- zabbix frontend, based on [zabbix/zabbix-web-apache-mysql:alpine-5.2.5](https://hub.docker.com/r/zabbix/zabbix-web-apache-mysql)
- zabbix-agent, based on [zabbix/zabbix-agent2:alpine-5.2.5](https://hub.docker.com/r/zabbix/zabbix-agent2)

Just run the following command in the folder where the docker-compose.yml file is located:

docker-compose up -d

After that you can reach web interface on port 8080:
http://your-raspberry-ip:8080
