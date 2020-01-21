## Kafka

```Java

C:\kafka_2.11-2.0.0\bin\windows

zookeeper-server-start.bat C:\kafka_2.11-2.0.0\config\zookeeper.properties

kafka-server-start.bat C:\kafka_2.11-2.0.0\config\server.properties

kafka-topics.bat --create --zookeeper localhost:2181 --replication-factor 1 --partitions 1 --topic helloTopic

kafka-console-producer.bat --broker-list localhost:9092 --topic helloTopic

kafka-console-consumer.bat --topic helloTopic --bootstrap-server localhost:9092

```

