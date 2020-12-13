# AWS Kinesis Overview

* Kinesis is a managed alternative to apache kafka
* Great for application logs, metrics IOT, clickstreams
* Great for real-time big data
* Great for straming processing frameworks(Spark, Nifi, etc...)
* Data is automatically replicated synchronosly to 3 AZ
  
## Services
* Kinesis Streams: low latency streaming ingest at scale
* Kinesis Analytics: perform real-time analytics on streams using SQL
* Kinesis Firehose: load streams into S3, Redshift, Elact

## Kinesis 

(click Stream,
IOT devices,
Metrics Logs )-> 
Kinesis Streams -> 
Kinesis Analytics -> 
Kinesis Firehose -> Amazon Red shit


### Kinesis Streams Overview

* Streams are divided in ordered Shards/Partitions
 producers --> [SHARD 1, SHARD 2, SHARD3] --> CONSUMERS
* Its stores the data for 24 hours, you can go up to 7 days
* Ability to reprocess/replay data
* Multiple application can consume the same stream 
* Real time processing with scale of throughput
* Once data is inserted in Kinesis, It can't be deleted 

### Kinesis Streams Shards
* One stream is make of many different shards
* Billing is per shard provisioned, can have as many shards as you want
* Batching available or per message calls



  
  

