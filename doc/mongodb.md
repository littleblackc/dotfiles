MongoDB
=======

#Install

###debian8
-----------
```
#aptitude install mongodb
# close inital start with system
# sysv-rc-conf change mongodb 2345
```


###debian7
-----------
```
#apt-key adv --keyserver keyserver.ubuntu.com --recv 7F0CEB10
#echo "deb http://repo.mongodb.org/apt/debian wheezy/mongodb-org/3.0 main" | tee /etc/apt/sources.list.d/mongodb-org-3.0.list
#apt-get update
#apt-get install -y mongodb-org
#apt-get install -y mongodb-org=3.0.7 mongodb-org-server=3.0.7 mongodb-org-shell=3.0.7 mongodb-org-mongos=3.0.7 mongodb-org-tools=3.0.7
#echo "mongodb-org hold" | sudo dpkg --set-selections
#echo "mongodb-org-server hold" | sudo dpkg --set-selections
#echo "mongodb-org-shell hold" | sudo dpkg --set-selections
#echo "mongodb-org-mongos hold" | sudo dpkg --set-selections
#echo "mongodb-org-tools hold" | sudo dpkg --set-selections
#sudo service mongod start
#cat /var/log/mongodb/mongod.log
#sudo service mongod stop
#sudo service mongod restart
#sudo apt-get purge mongodb-org*
#sudo rm -r /var/log/mongodb
#sudo rm -r /var/lib/mongodb
```
