# Домашнее задание к занятию "Система мониторинга Zabbix" - `Ерофеев Максим`


### Задание 1
![Удачная установка](https://github.com/ErofeevMA-Git/hw-02/blob/main/img/zabbix1.jpg)
![Авторизация](https://github.com/ErofeevMA-Git/hw-02/blob/main/img/zabbix2.jpg)
![Главная страница](https://github.com/ErofeevMA-Git/hw-02/blob/main/img/zabbix3.jpg)

# Команды для установки Zabbix сервера и PostgreSQL 
- sudo -s
- wget https://repo.zabbix.com/zabbix/7.4/release/ubuntu/pool/main/z/zabbix-release/zabbix-release_latest_7.4+ubuntu24.04_all.deb
- dpkg -i zabbix-release_latest_7.4+ubuntu24.04_all.deb
- apt update
- apt install zabbix-server-pgsql zabbix-frontend-php php8.3-pgsql zabbix-apache-conf zabbix-sql-scripts
- sudo -u postgres createuser --pwprompt zabbix
- sudo -u postgres createdb -O zabbix zabbix
- systemctl restart zabbix-server apache2
- systemctl enable zabbix-server apache2
# Команды Git
- git clone
- git add .
- git commit -m "Update"
- git push origin main
  
### Задание 2
![Hosts](https://github.com/ErofeevMA-Git/hw-02/blob/main/img/zabbix4.jpg)
![Logs](https://github.com/ErofeevMA-Git/hw-02/blob/main/img/zabbix5.jpg)
![Latest](https://github.com/ErofeevMA-Git/hw-02/blob/main/img/zabbix6.jpg)

# Команды для установки Zabbix агента
- sudo -s
- wget https://repo.zabbix.com/zabbix/7.4/release/ubuntu/pool/main/z/zabbix-release/zabbix-release_latest_7.4+ubuntu24.04_all.deb
- dpkg -i zabbix-release_latest_7.4+ubuntu24.04_all.deb
- apt update
- apt install zabbix-agent
- systemctl restart zabbix-agent
- systemctl enable zabbix-agent
# Команды Git
- git clone
- git add .
- git commit -m "Update"
- git push origin main
