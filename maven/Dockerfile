FROM ubuntu:18.04
RUN apt update && \
apt install default-jdk -y && \
apt install maven -y && \
apt install git -y && \
mkdir /home/$USER/GIT
WORKDIR /home/$USER/GIT
RUN git clone https://github.com/boxfuse/boxfuse-sample-java-war-hello.git
WORKDIR  /home/$USER/GIT/boxfuse-sample-java-war-hello
RUN mvn package  
CMD tail -f /dev/null
