

```
$ sudo apt install apache2
or
$ sudo apt-get install apache2


$ apache2 -v


apache2 -V


# apachectl configtest
or
# apachectl -t
or
# apache2ctl configtest
or
# apache2ctl -t

$ apache2ctl -S
or
$ apachectl -S

# systemctl start apache2  		[To Start the Apache2 Service]
# systemctl stop apache2		[To Stop the Apache2 Service]
# systemctl restart apache2		[To Restart the Apache2 Service]
# systemctl reload apache2		[To Reload the Apache2 Service]
# systemctl status apache2		[To Status the Apache2 Service]
# systemctl enable apache2		[To Enable the Apache2 Service]


$ sudo a2ensite xxxx.conf	[To Enable a New Website]
$ sudo a2dissite xxxx.conf	[To Disable a Website]


$ sudo a2enmod [Module]		[To Enable a New Module]
$ sudo a2dismod [Module]	[To Disable a Module]
$ sudo systemctl reload apache2


 apachectl -M
$ apache2ctl -M
$ a2query -m

$ ls -lh /usr/lib/apache2/modules/	[To List Available Modules]
$ ls -lh /etc/apache2/mods-available/	[To List Available Modules]
$ ls -lh /etc/apache2/mods-enabled/	[To List Enabled Modules]
$ ls -lh /var/www/html			[Apache2 Default Web root]
$ ls -lh /var/www/			[Other Website Web root]
$ less /etc/apache2/apache2.conf	[Apache2 Main Configuration File]
$ less /etc/apache2/ports.conf		[Apache2 Ports Configuration File]
$ less /var/log/apache2/error.log	[Apache2 Error Log File]
$ less /var/log/apache2/access.log	[Apache2 Access Log File]


# ss -ant | grep :80 | wc -l
or
# netstat -ant | grep :80 | wc -l
90

```