FROM tomcat:8.0
RUN apt-get update -y
RUN curl -L -O https://artifacts.elastic.co/downloads/beats/filebeat/filebeat-6.3.2-amd64.deb
RUN dpkg -i filebeat-6.3.2-amd64.deb
COPY ./filebeat/filebeat.yml /etc/filebeat
RUN service filebeat start
#RUN filebeat modules enable system

