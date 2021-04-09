FROM ubuntu:latest
RUN ln -snf /usr/share/zoneinfo/Europe/Moscow /etc/localtime ;\
apt update -y ;\
apt install git -y;\
apt update -y ;\
apt install maven -y ;\
apt update -y 

WORKDIR /home/user/
RUN git clone https://github.com/boxfuse/boxfuse-sample-java-war-hello.git ./;\
mvn package 
RUN ["/bin/bash"]
#/home/user/target#

#RUN cp /home/user/boxfuse-sample-java-war-hello/target/hello-1.0.war "$CATALINA_HOME"/webapps/



