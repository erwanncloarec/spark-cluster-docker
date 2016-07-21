FROM java:8

MAINTAINER Erwann CLOAREC <ecloarec@cyres.fr>

ADD http://d3kbcqa49mib13.cloudfront.net/spark-1.6.2-bin-hadoop2.6.tgz /opt/

RUN cd /opt && tar -xzf spark-1.6.2-bin-hadoop2.6.tgz && rm spark-1.6.2-bin-hadoop2.6.tgz && mv spark-1.6.2-bin-hadoop2.6 spark

WORKDIR /opt/spark

ENTRYPOINT ["bin/spark-class", "org.apache.spark.deploy.worker.Worker"]
