# Big Data — Spark & PySpark Projects

Distributed data processing projects built with **PySpark on Databricks**, covering batch ML, graph-based recommendations, and real-time streaming.

## Projects

| # | Project | Description | Demo |
|---|---|---|---|
| 1 | **Movie Search Engine by Plot** | TF-IDF search over movie plot summaries — query any description, get ranked matches | [Databricks notebook](https://databricks-prod-cloudfront.cloud.databricks.com/public/4027ec902e239c93eaaa8714f173bcfc/1909261951439895/2513447359152657/4943942562258491/latest.html) |
| 2 | **Friend Recommendation System** | Graph-based mutual-friend recommendations over a social network dataset, MapReduce-style | [Databricks notebook](https://databricks-prod-cloudfront.cloud.databricks.com/public/4027ec902e239c93eaaa8714f173bcfc/1909261951439895/2502237766088152/4943942562258491/latest.html) |
| 3 | **Naive Bayes — from scratch** | Classifier implemented directly in PySpark primitives (no ML libraries) | [Databricks notebook](https://databricks-prod-cloudfront.cloud.databricks.com/public/4027ec902e239c93eaaa8714f173bcfc/1909261951439895/1924594202234242/4943942562258491/latest.html) |
| 4 | **Naive Bayes — MLlib** | Same task via Spark MLlib, for comparison of accuracy and code complexity | [Databricks notebook](https://databricks-prod-cloudfront.cloud.databricks.com/public/4027ec902e239c93eaaa8714f173bcfc/1909261951439895/3183337138173317/4943942562258491/latest.html) |
| 5 | **WordCount for Named Entities** | Entity extraction + distributed counting over a large text corpus | — |
| 6 | **Movie Recommendation System** | Collaborative filtering with Spark | — |
| 7 | **Spark Streaming + Kafka** | Real-time pipeline: Kafka ingestion → Spark Streaming → ELK stack | — |

## Stack

PySpark · Databricks · Spark MLlib · Kafka · Elasticsearch/Logstash/Kibana

## Notes

Built during my MS at UT Dallas (Big Data Management & Analytics). The from-scratch vs MLlib Naive Bayes pair (#3/#4) is the most interesting read — it shows what the framework abstracts away.
