FROM 		tomcat:8.0
MAINTAINER 	Kevin Daniel Pinchi García (kevin.pinchi.garcia@gmail.com)
COPY 		./shared/sample.war /usr/local/tomcat/webapps/
RUN             mkdir /opt/shared
RUN		echo "Hola mundo" >> /opt/hola_mundo.txt
COPY            ./shared/Context.xml /opt/shared/
COPY            ./shared/tomcat-users.xml /opt/shared/
RUN             apt-get clean && rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
