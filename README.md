I disabled any sync folder between host and VM. For better perf, you should ask your IDE to push files by SFTP 
using the generated ssh key in puphpet\files\dot\ssh folder.

You should change the host in the file "puphpet/config.yaml" or reimport it in puphpet.com and change whatever 
your need.

You use this configuration for many project, works on all OS and it's so fast!

You might need to change the permission of the web folder. You have to deploy your code into /var/www/dev.

You tend to use one VM per project ;)

have a look to nginx configuration. It's still not optimal and useable after first vagrant up. Need to fix something.



MYSQL
======

[mysqld]
bind-address = 0.0.0.0
#skip-external-locking
#skip-external-locking 
#bind-address