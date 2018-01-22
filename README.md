# Linux-Server-configuration
Udacity project for deploying web application on a configured Amazon lightsail web server

IP address: 18.218.112.221
SSH port: 2200
URL of hosted application: http://ec2-18-218-112-221.us-east-2.compute.amazonaws.com/
1- Configuration changes made:

-Changed SSH port to 2200
-Created user grader and provided him sudo access.
-Set the timezone to UTC
-Created a catalog user for accessing the database
-Installed mod_wsgi, postgresQL and installed and configured the catalogwithmenusers database
- Cloned and setup the catalog item web application

-ubuntu@ip-172-26-15-147:/var/www/html/catalog$ sudo ufw status
Status: active

To                         Action      From
--                         ------      ----
2200/tcp                   ALLOW       Anywhere
22/tcp                     DENY        Anywhere
123                        ALLOW       Anywhere
80                         ALLOW       Anywhere
2200/tcp (v6)              ALLOW       Anywhere (v6)
22/tcp (v6)                DENY        Anywhere (v6)
123 (v6)                   ALLOW       Anywhere (v6)
80 (v6)                    ALLOW       Anywhere (v6)

2- Software (packages) installed:

asn1crypto==0.24.0
autopep8==1.3.2
backports.shutil-get-terminal-size==1.0.0
certifi==2017.11.5
cffi==1.11.4
chardet==3.0.4
click==6.7
configparser==3.5.0
cryptography==2.1.4
enum34==1.1.6
flake8==3.5.0
Flask==0.12.2
google-api-python-client==1.6.5
gunicorn==19.7.1
httplib2==0.10.3
idna==2.5
ipaddress==1.0.19
itsdangerous==0.24
Jinja2==2.10
MarkupSafe==1.0
mccabe==0.6.1
oauth2==1.9.0.post1
oauth2client==4.1.2
pathlib==1.0.1
pep8==1.7.0
pew==1.1.1
pipenv==8.3.2
psutil==5.3.1
psycopg2==2.7.3.2
pyasn1==0.4.2
pyasn1-modules==0.2.1
pycodestyle==2.3.1
pycparser==2.18
pyflakes==1.6.0
PyJWT==1.5.3
pyOpenSSL==17.0.0
pytz==2017.3
requests==2.18.4
rsa==3.4.2
shutilwhich==1.1.0
six==1.11.0
SQLAlchemy==1.1.15
twilio==6.4.1
uritemplate==3.0.0
urllib3==1.22
virtualenv==15.1.0
virtualenv-clone==0.2.6
Werkzeug==0.13


2- Third-party resources used for completing the project
- http://flask.pocoo.org/docs/0.10/deploying/mod_wsgi/
- https://aws.amazon.com/premiumsupport/knowledge-center/new-user-accounts-linux-instance/
- https://www.digitalocean.com/community/tutorials/how-to-install-linux-apache-mysql-php-lamp-stack-on-ubuntu-14-04
