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

Mahout :- Machine Learning Library 

-------------------------------------------------------

HDFS
30-05-2017 

1) Example we have blocks called chunks mydata.txt 
File is split into chunks which is called blocks

2) Default block size is 64MB , each block is given a unique name blk_1 , blk_2 etc 

example 150mb file 64Mb + 64Mb + 22Mb , each block will get stored in one node in the cluster .

DataNode :- there is a daemon that is running in all the machine in the cluster. 

NameNode :- daemon knows which chunks make up which file. 
(It has metadata).

Some Problems encountered

a) Network Failure.
b) Disk Failure on DiskNode.
c) Disk Failure on NameNode.


Data Redundancy, Hadoop replicated each block 3 times, 
When the namenode sees that the blocks have not been replicated, it will make sure that they are replicated.

---------------------------------------------------------

NameNode High Availability 

Namenode needs to copied on the network NFS. Sometime 2 Namenode are configured (Active) and (Standby).




