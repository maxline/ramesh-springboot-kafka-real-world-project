## RameshMF Spring Boot and Apache Kafka course with real project example

- https://udemy.com/course/spring-boot-and-apache-kafka
- https://github.com/RameshMF/springboot-kafka-course
- https://kafka.apache.org/quickstart

## Terminal kafka commands
$ cd kafka
$ bin/kafka-storage.sh format --standalone -t $KAFKA_CLUSTER_ID -c config/server.properties

$ bin/kafka-server-start.sh config/server.properties           
$ bin/kafka-console-consumer.sh --topic javaguides_json --from-beginning --bootstrap-server localhost:9092
$ bin/kafka-console-consumer.sh --topic wikimedia_recentchange --from-beginning --bootstrap-server localhost:9092

## Project api
### Simple String message
http://localhost:8080/api/v1/kafka/publish?message=hello%20Anton11

### Json message
POST (Talent Api Tester)
http://localhost:8080/api/v1/kafka/user-publish
```
{
"id": "1",
"firstName": "Mike3",
"secondName": "NY"
}
```

## wikimedia api
- https://stream.wikimedia.org/v2/stream/recentchange

## Database 
```
SELECT * FROM wikimedia.wikimedia_recentchange;
```
## Useful config settings
logging.level.org.springframework.web: DEBUG

