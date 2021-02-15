FROM ubuntu:18.04
RUN apt-get update && apt-get install default-jdk -y && apt-get install git -y && apt-get install maven -y
WORKDIR /tmp/
RUN git clone https://github.com/boxfuse/boxfuse-sample-java-war-hello.git
WORKDIR /tmp/boxfuse-sample-java-war-hello/
RUN mvn package