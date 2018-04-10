* CPU Utilization
    * Memcached, multi-threaded, can handle loads of up to 90%.  If it exceeeds 90%, add more nodes to the cluster
    * Redis, not multi-threaded.  To determine the point in which to scale, take 90 and divide by the number of cores (not needed for exam)
* Swap Usage
    * swap usage is simple the amount of the swap file that is used
    * memcached, should be 0 most of the time, if exceeds 50Mb, increase memcached_connections_overhead parameter
    * redis, no SwapUsage metric
* Evictions
    * when a new item is added and an old item must be removed
    * memcached, there is no recommended setting. Tweak based on application requirements, scale up or out
    * redis, only scale out
* Concurrent Connections
    * No recommended setting.  Set an alarm on the number of concurrent connections for elasticache
    * make sure application is releasing connections as it should be
