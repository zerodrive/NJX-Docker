# Use this image as basis for our container.
FROM tomcat:8.0
#
# This is optional. There are many other LABELs possible.
LABEL maintainer "thomas.schwade@zerodrive.net"
#
# The tomcat:8.0 image contains the tomcat files under /usr/local/tomcat.
# We provide our own tomcat-users.xml file with a predefined administrator account.
# We can of course provide any other specific configuration file too.
COPY tomcat-users.xml /usr/local/tomcat/conf/tomcat-users.xml
#
# We deploy our web application.
COPY NaturalAjaxDemos.war /usr/local/tomcat/webapps
