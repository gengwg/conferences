DataStax Solution Day  
San Francisco, April 25 2018

core dse
========
```
ring
coordinator node
datastax academy 201 course

rf = 2
each node has 2 partition ranges

multi-dc replication

rf: copies of data
cl: how many nodes going to respond.

cl = quorum
use most recent one.

cl = all
if one node fails, read fail.

strong consistency
w cl = all
r cl = one
OR:
w cl = quorum
r cl = quorum

log-structure

ciurclular log storage
make the previous version invalid 
compactor defrag storage

memtable in ram, sorted by clustering column.
commit log on hdd, appened
when full, delete commit log. write to SSTable (immutable).
when read find multiple SSTable and read latest, because SSTable not immutable.

partition index on disk
token --> byte offset

optimization: 
partition summary in ram
keyCache
bloom filter 

read gets entire partition
partition is unit of access
partition key --> hash function --> partition token
associate rows with
    clustoering columns
    data columns

primary key = ((partition key), clustering columns)
must supply partition key
```

graph
=====

graph not have to be on each node, unlike neojs.

