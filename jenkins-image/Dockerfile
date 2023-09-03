FROM ubuntu
RUN apt-get update -y
RUN apt-get install openjdk-8-jre -y
RUN echo "JAVA_HOME=/usr/" >> ~/.bashrc
ADD https://dlcdn.apache.org/tomcat/tomcat-9/v9.0.80/bin/apache-tomcat-9.0.80.tar.gz /tmp
RUN cd /tmp && tar -xvzf apache-tomcat-9.0.80.tar.gz
RUN cd /tmp && mv apache-tomcat-9.0.80.tar.gz /opt/
EXPOSE 8080
ADD https://get.jenkins.io/war-stable/latest/jenkins.war /opt/apache-tomcat-9.0.80/webapps/