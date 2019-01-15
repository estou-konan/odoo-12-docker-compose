# Usage

Download folder "odoo-12-docker-compose" to your PC then Open Terminal at same above folder path. 


# Folder Permission :
Change the folder permission to make sure that the container is able to access the directory:
```
$ sudo chmod -R 777 addons
$ sudo chmod -R 777 etc
```
# Odoo Port
Edit file docker-compose.yml and change Odoo port from 8071 to any un-use port or keep it.
```
ports:
 - "8071:8069"
```

# Custom addons
The **addons** folder contains custom module. Just put your custom module if you have any.

# Run Odoo Server
For first time only run the following command to ensure the setup of new configuration:
```
$ docker-compose config
```
To start the container, execute this command:
```
$ docker-compose up
```
To run in detached mode, execute this command:
```
$ docker-compose up -d
```

# Odoo Logs
* Log file is printed @ **etc/odoo-server.log**


# Odoo configuration

To change Odoo configuration, edit file: **etc/odoo.conf**.

# docker-compose.yml

* odoo:12.0
* postgres:9.5

# Odoo 12 screenshots

![odoo-12-welcome-docker](screenshots/odoo-12-welcome-screenshot.png)

![odoo-12-apps-docker](screenshots/odoo-12-apps-screenshot.png)

![odoo-12-sales](screenshots/odoo-12-sales-screen.png)
