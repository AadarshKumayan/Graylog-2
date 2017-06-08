# Graylog-2
setting up a graylog server on a virtual machine

USE ORACLE JDK 1.8 instead of openjdk if getting java exceptions or error on login 


commands-

cat CentOS-Base.repo

sudo rpm -Uvh https://packages.graylog2.org/repo/packages/graylog-collector-latest-repository-el7_latest.rpm

yum install graylog-collector

yum install ntp

time

date

chkconfig ntpd on

ntpdate pool.ntp.org

service ntpd start

date

vi /etc/sysconfig/clock

yum install update

yum update

yum install java-1.8.0-openjdk-headless.x86_64

yum install epel-release

yum install pwgen

pwen 10 1

clear

cd /etc/yum.repos.d

ls

vi mongodb-org-3.2.repo

yum install mongodb-org

chkconfig --add mongod

systemctl daemon-reload

systemctl enable mongod.service

systemctl start mongod.service

systemctl mongod.service status

systemctl mongod status

service mongod status

rpm --import https://packages.elastic.co/GPG-KEY-elasticsearch

vi elasticsearch.repo

yum install elastic serach

yum install elasticsearch

vi elasticsearch.repo

yum install elasticsearch

vi /etc/elastic/search/elasticsearch.yml

cd /etc/elasticsearch

ls

cat elasticsearch.yml

vi elasticsearch.yml

chkconfig --add elasticsearch

systemctl daemon-reload

systemctl enable elasticsearch.service

systemctl restart elasticsearch.service

service elasticsearch status

rpm -Uvh https://packages.graylog2.org/repo/packages/graylog-2.2repository_latest.rpm

rpm -Uvh https://packages.graylog2.org/repo/packages/graylog-2.2-repository_latest.rpm

yum install graylog-server

chkconfig --add graylog-server

systemctl daemon-reload

systemctl enable graylog-server.service

systemctl restart graylog-server.service

systemctl status graylog-server.service

if service starts running the type server ip :port in url tu see web ui 


