sudo yum update -y && sudo yum install httpd php git -y && sudo service httpd start && sudo chkconfig httpd on &&  cd /var/www/html  && sudo git clone https://github.com/git786hub/sampleawsphpdb.git  &&  cd sampleawsphpdb && sudo cp be.sh /var/www/html && cd /var/www/html &&  sudo ./be.sh


to change php version ( 5to 7 )

[ec2-user@ip-172-31-12-233 ~]$ php -v

PHP 5.4.16 (cli) (built: Sep  1 2018 05:47:37)
Copyright (c) 1997-2013 The PHP Group
Zend Engine v2.4.0, Copyright (c) 1998-2013 Zend Technologies

[ec2-user@ip-172-31-12-233 ~]$  sudo yum remove php-common mod_php php-cli -y

[ec2-user@ip-172-31-12-233 ~]$ sudo -i

[root@ip-172-31-12-233 ~]#  yum install https://dl.fedoraproject.org/pub/epel/epel-release-latest-7.noarch.rpm -y

[root@ip-172-31-12-233 ~]#  yum install http://rpms.remirepo.net/enterprise/remi-release-7.rpm -y


[root@ip-172-31-12-233 ~]#  sudo amazon-linux-extras install php7.1 -y

[root@ip-172-31-12-233 ~]# php -v

PHP 7.1.30 (cli) (built: Jun 12 2019 20:33:42) ( NTS )
Copyright (c) 1997-2018 The PHP Group
Zend Engine v3.1.0, Copyright (c) 1998-2018 Zend Technologies

.
