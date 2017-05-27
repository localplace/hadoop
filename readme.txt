HADOOP - THEORY

27 - May - 2017

Store and process large amounts of data 
process across many machines

-------------------------------------------------------

3vs

Volume :- Size of data 

Variety :- data is coming from different sources with different formats (structured and unstructured data)

unstructured data :- text, mp3, store date in raw format 

Velocity :- the speed at which its getting generated 
Rate of terabytes 
--------------------------------------------------------


HADOOP

Store Data :- HDFS (Hadoop Distributed File System) .

Split the data and store it in a cluster of machines call the CLUSTER 

Process Data :- MapReduce 
-------------------------------------------------------

HADOOP ECOSYSTEM

HIVE :- Looks like SQL, Hive Interpreter will turn sql to 
MAP REDUCE code 

PIG :- Scripting language -> converts to mapreduce

IMPALA :- Directly access HDFS rather than mapreduce. Low Latency queries 

Sqoop :- Traaditional SQL to HDFS 

Flume :- Injects data from external systems and puts into the cluster

HBase :- Real time database on top of HDFS

Mahout :- Machine Learnign Library 

-------------------------------------------------------




