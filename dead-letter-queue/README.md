# Dead Letter Queue

Creates two Kafka brokers, kafka-source (mapped to 9091) and kafka-target (mapped to 9092)
Creates Kafka Connect, attached to kafka-source

Installs a single simple FileStreamSinkConnector with a dead letter queue (DLQ) in kafka-target.
Source topic and connect configurations are in kafka-source

The output of the connector will be written into an output directory.
