# Overview

All notes derived from http://crunch.apache.org/

## Introduction
* Apache Crunch runs on top of Hadoop MapReduce and Apache Spark
* Apache Crunch is a simple Java API for performing tasks like data aggregation and joins which are hard to implement in plain MapReduce thus simplifying the process of creating data pipelines on top of Apache Hadoop.
* This API is useful when processing data cannot be used out of the box / does not fit into the relational models (e.g. time series) OR serialized object formats (e.g. protocol buffers, Avro Records) OR HBase rows & columns.
