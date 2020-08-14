# Kafka Stack Cluster
This setup runs a 3:1 kafka cluster (3 broker, 1 zookeeper).

#### Included
- Kafka (3)
- Zookeeper (1)
- Schema registry
- Kafka connect
- Rest proxy
- Kafka manager
- Connect UI
- Schema registry UI

#### Pre
Change {HOST_IP} with your machine's IP address.

#### Setup

1. Move to kafka-cluster directory and execute
```bash
docker-compose up -d
```

2. Then move to kafka-stack directory and execute
```bash
docker-compose up -d
```

#### Cleanup

1. Move to kafka-stack directory and execute
```bash
docker-compose down
```

2. Then move to kafka-cluster directory and execute
```bash
docker-compose down
```

#### Ports
- Kafka: 9092-9094
- Zookeeper: 2181
- Schema registry: 8081
- Kafka connect: 8083
- Rest proxy: 8084
- Kafka manager: 9000
- Connect UI: 8001
- Schema registry UI: 8002

These ports should be accessible

#### Storage
Data are stored in `storage` folder of each directory.
