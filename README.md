# flume-kafka

KAFKA ON ITVERSITY LAB


first add environment varibales to .bash_profile

export KAFKA_HOME=/usr/hdp/2.5.0.0-1245/kafka
PATH=$PATH:$KAFKA_HOME/bin

export PATH

creating Topic

kafka-topics.sh --create \
--zookeeper nn01.itversity.com:2181,nn02.itversity.com:2181,rm01.itversity.com \
--replication-factor 1 \
--partitions 1 \
--topic jaykafaka1

creating producer

kafka-console-producer.sh \
> --broker-list nn02.itversity.com:6667 \
> --topic jaykafaka1

type messages after the topic,, the messages will be stored on the host while brokers are running


creating consumer




