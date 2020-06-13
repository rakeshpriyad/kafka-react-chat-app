# Chat Application
A Realtime Chat Application built using React and Kafka as MessageBroker




## Before Running the Project 

*Start Zookeeper*
```shell script
.\bin\windows\zookeeper-server-start .\config\zookeeper.properties
```

*Start Kafka*
```shell script
.\bin\windows\kafka-server-start .\config\server.properties
```

*Create a Topic*
```
.bin\windows\kafka-topics --create --topic kafka-chat --zookeeper localhost:2181 --replication-factor 1 --partitions 1
```

*Start Backend*
```
mvn spring-boot:run
```

*Start Frontend*
```
npm start
```
Open two browser
login with any name in both browser
http://localhost:3000/
http://localhost:3000/

Start typing messages


