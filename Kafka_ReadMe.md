## Kafka

```Java

C:\kafka_2.11-2.0.0\bin\windows

zookeeper-server-start.bat C:\kafka_2.11-2.0.0\config\zookeeper.properties

kafka-server-start.bat C:\kafka_2.11-2.0.0\config\server.properties

kafka-topics.bat --create --zookeeper localhost:2181 --replication-factor 1 --partitions 1 --topic helloTopic

kafka-console-producer.bat --broker-list localhost:9092 --topic helloTopic

kafka-console-consumer.bat --topic helloTopic --bootstrap-server localhost:9092

```

* To Refer More details : https://dzone.com/articles/magic-of-kafka-with-spring-boot

#### Steps to implements Kafka

* Download Kafka from : https://kafka.apache.org/quickstart

* Before running application follow below steps

  * Go to C:\kafka_2.11-2.0.0\bin\windows  folder using CMD and 
  * You can name every CMD winodw "title name" command
  * Start ZooKeeper : zookeeper-server-start.bat C:\kafka_2.11-2.0.0\config\zookeeper.properties
  * Start Server : kafka-server-start.bat C:\kafka_2.11-2.0.0\config\server.properties
  * Create Topic : kafka-topics.bat --create --zookeeper localhost:2181 --replication-factor 1 --partitions 1 --topic helloTopic
  * Start Producer :kafka-console-producer.bat --broker-list localhost:9092 --topic helloTopic
  * Now you can produce all messages either application or producer console
  * Start Consumer : kafka-console-consumer.bat --topic helloTopic --bootstrap-server localhost:9092 to get all produced messages from the topic.
  
  
  
  


