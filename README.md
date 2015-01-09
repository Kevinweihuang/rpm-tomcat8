rpm-tomcat7
===========

An RPM spec file to install Tomcat 7.0.

To Build:

`sudo yum -y install rpmdevtools && rpmdev-setuptree`

`wget https://raw.github.com/nmilford/rpm-tomcat7/master/tomcat7.spec -O ~/rpmbuild/SPECS/tomcat7.spec`

`wget https://raw.github.com/nmilford/rpm-tomcat7/master/tomcat7.init -O ~/rpmbuild/SOURCES/tomcat7.init`

`wget https://raw.github.com/nmilford/rpm-tomcat7/master/tomcat7.sysconfig -O ~/rpmbuild/SOURCES/tomcat7.sysconfig`

`wget https://raw.github.com/nmilford/rpm-tomcat7/master/tomcat7.logrotate -O ~/rpmbuild/SOURCES/tomcat7.logrotate`

`wget http://www.motorlogy.com/apache/tomcat/tomcat-7/v7.0.55/bin/apache-tomcat-7.0.55.tar.gz -O ~/rpmbuild/SOURCES/apache-tomcat-7.0.55.tar.gz`

`rpmbuild -bb ~/rpmbuild/SPECS/tomcat7.spec`

根据centos环境下的tomcat6 做了一点调整，同时增加了/usr/sbin/tomcat7 脚本
