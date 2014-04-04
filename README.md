rpm-tomcat7
===========

An RPM spec file to install Tomcat 7.0. Designed to be as similar to the
stock EL6 tomcat6 package as possible.

To Build:

`sudo yum -y install rpmdevtools && rpmdev-setuptree`

`wget https://raw.github.com/nmilford/rpm-tomcat7/master/tomcat7.spec -O ~/rpmbuild/SPECS/tomcat7.spec`

`wget https://raw.github.com/nmilford/rpm-tomcat7/master/tomcat7.init -O ~/rpmbuild/SOURCES/tomcat7.init`

`wget https://raw.github.com/nmilford/rpm-tomcat7/master/tomcat7.sysconfig -O ~/rpmbuild/SOURCES/tomcat7.sysconfig`

`wget https://raw.github.com/nmilford/rpm-tomcat7/master/tomcat7.logrotate -O ~/rpmbuild/SOURCES/tomcat7.logrotate`

`wget http://www.motorlogy.com/apache/tomcat/tomcat-7/v7.0.53/bin/apache-tomcat-7.0.53.tar.gz -O ~/rpmbuild/SOURCES/apache-tomcat-7.0.53.tar.gz`

`rpmbuild -bb ~/rpmbuild/SPECS/tomcat7.spec`
