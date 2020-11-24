FROM        127.0.0.1:5000/centos:7
MAINTAINER  machard.1984@gmail.com
RUN         wget -P /etc/yum.repos.d/ http://10.0.33.55/repository/configs/yum.repos.d/epel.repo
RUN         yum install -y -q python3-flask
RUN         pip3 install flask-restful pymongo pyOpenSSL
ADD         py/api /usr/bin/
ENTRYPOINT  ["/usr/bin/api"]
