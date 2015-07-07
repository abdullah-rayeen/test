#Docker container for Magento environment

##Steps

1. Create magento folder under data/srv and copy Magento source files/folders under data/srv/magento folder
Download the magento release archives from here:
```sh
https://www.magentocommerce.com/download
```
2. Reset Magento files and folders permission:
```sh
$ chmod -R 0777 var/
$ chmod -R 0777 media/
```

3.Install docker and fig onto host machine

4. Build the containers
```sh
$ fig build
```
5. Up the containers daemonize
```sh
$ fig up -d
```

6. Open http://localhost:80 onto browser

7. Move ahead with the magento installation steps

8. Enter mysql connections while Magento installation:
Host: <mysql container IP>
Database: <create a DB after bash to the mysql container>
User: <create a mysql user after bash to the mysql container and grant full access to the Magento DB>
Password: <Use the same password used while create Magento DB user>

9. Complete the Magento installation steps

10. Its All done!!!