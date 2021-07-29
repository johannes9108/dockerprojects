#COMMENT
FROM ubuntu
RUN mkdir -p /home/kafka
RUN mkdir /usr/local/java
COPY ./kafka_2.12-2.8.0 /home/kafka/
COPY jre-8u291-linux-x64.tar.gz /usr/local/java
WORKDIR /usr/local/java
RUN tar zxvf ./jre-8u291-linux-x64.tar.gz
RUN rm jre-8u291-linux-x64.tar.gz
RUN update-alternatives --install "/usr/bin/java" "java" "/usr/local/java/jre1.8.0_291/bin/java" 1
WORKDIR /home/kafka
#apt-get update