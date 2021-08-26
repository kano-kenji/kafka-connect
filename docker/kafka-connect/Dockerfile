FROM confluentinc/cp-kafka-connect:6.2.0

USER 0
RUN yum install unzip -y
RUN mkdir -p /usr/share/java/

WORKDIR /

# debezium-connector-sqlserver
RUN wget https://repo1.maven.org/maven2/io/debezium/debezium-connector-sqlserver/1.6.0.Final/debezium-connector-sqlserver-1.6.0.Final-plugin.tar.gz -O /tmp/debezium-connector-sqlserver.tar.gz \
&& tar -xvzf /tmp/debezium-connector-sqlserver.tar.gz --directory /usr/share/java/ \
&& rm /tmp/debezium-connector-sqlserver.tar.gz