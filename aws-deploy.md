# AWS Deployement

```shell
# Tunneling ssh
ssh grp02@52.41.239.75 -L 23:10.0.02.10:22 -i GRP02.pem

# SSH to appli server
ssh admin@localhost -p 23 -i I239_GRP02_APPLI_SRV.pem

#Tunneling HTTP 8181 -> 8080
ssh grp02@52.41.239.75 -L 8181:10.0.02.10:8080 -i GRP02.pem

#Tunneling MySQL 3307 -> 3306
ssh grp02@52.41.239.75 -L 3307:10.0.02.10:3306 -i GRP02.pem
```


pour désinstaller mariadb entièrement.
sudo apt remove mariadb-server
sudo apt purge mariadb-server

sudo systemctl stop mysql
sudo rm -rf /var/lib/mysql/*
sudo systemctl start mysql

uninstall.

