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
  
##### Step1 Start Zookeeper

  ![ZooKeeper](https://github.com/privatevkakarla/project8-vkakarla-springboot-kafka-producer-consumer-service/blob/master/src/main/resources/Images/ZooKeeper.PNG "ZooKeeper")
  
##### Step2 Start Server

  ![Server](https://github.com/privatevkakarla/project8-vkakarla-springboot-kafka-producer-consumer-service/blob/master/src/main/resources/Images/Server.PNG "Server")  

##### Step3 Create Topic

  ![Topic](https://github.com/privatevkakarla/project8-vkakarla-springboot-kafka-producer-consumer-service/blob/master/src/main/resources/Images/Topic.PNG "Topic") 
  
 ##### Step4 Start Producer

  ![Producer](https://github.com/privatevkakarla/project8-vkakarla-springboot-kafka-producer-consumer-service/blob/master/src/main/resources/Images/Producer.PNG "Producer")
  
 ##### Step5 Start Consumer

  ![Consumer](https://github.com/privatevkakarla/project8-vkakarla-springboot-kafka-producer-consumer-service/blob/master/src/main/resources/Images/Consumer.PNG "Consumer") 
  
  
##### Once you published the messages in topic and consumed from the topic by the consumer

  ![ConsoleOutput](https://github.com/privatevkakarla/project8-vkakarla-springboot-kafka-producer-consumer-service/blob/master/src/main/resources/Images/ConsoleOutput.PNG "ConsoleOutput")   
   
  
