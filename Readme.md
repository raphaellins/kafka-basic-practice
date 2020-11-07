First of all

    Download Kafka => https://kafka.apache.org/downloads

Start Zookeeper (service discovery)

    bin/zookeeper-server-start.sh config/zookeeper.properties

Start Kafka server

    bin/kafka-server-start.sh config/server.properties

Create a Kafka Topic

    bin/kafka-topics.sh --create --zookeeper localhost:2181 --replication-factor 1 --partitions 1 --topic Kafka_Example

Start the consumer to listen

    bin/Kafka-console-consumer.sh --bootstrap-server localhost:9092 --topic test --from-beginning