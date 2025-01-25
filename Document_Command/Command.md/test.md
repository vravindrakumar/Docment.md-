#!/bin/bash
sudo su
yum update -y
yum install -y httpd.X86_64

echo"<h1>Hello -Demo of User Data Script Amazon Linux| from $(hostname -f)<h1>" > /var/www/html/index.html/index
systemctl stop httpd.service
systemctl start httpd.service