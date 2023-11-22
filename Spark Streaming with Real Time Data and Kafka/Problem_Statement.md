
In this part, you will create a Spark Streaming application that will continuously read text data from a real time source, analyze the text for named entities, and send their counts to Apache Kafka. A pipeline using Elasticsearch and Kibana will read the data from Kafka and analyze it visually.

# Initial Setup: 
### NEWSAPI
```
NewsAPI - You can download real time news using the News API available at: https://newsapi.org/. There is also a Python wrapper for this available at: https://newsapi.org/docs/client-libraries/python
```

### APACHE KAFKA
```
Download Apache Kafka and go through the quickstart steps:
     https://kafka.apache.org/quickstart

```

### EKL Stack - Elastic Search, Kibana and Logstash 
```
Later, you will also need to set up Elasticsearch and Kibana environment to visualize data. You will need to download Elasticsearch, Kibana, and Logstash from https://www.elastic.co/downloads/

```