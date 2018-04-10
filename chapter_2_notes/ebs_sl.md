4 different types of EBS Storage
    general purpose (SSD) - gp2
        most workloads, system boot volumes, virt desktops, dev/test
        3 IOPS / GiB, Max size of volume is 16TiB, can burst up to 3000 with IO credits
        Need more than 3000 IOPS, increase volume size
    provisioned IOPS (SSD) - io1
        critical business, sustained IOPS, 100,000 IOPS or 160MiBs/s of throughput, Mongo, Cassandra, MySQL, etc.
    throughput optimized (HDD) - st1
        streaming workloads, log processing, big data, can't be a boot volume
    cold (HDD) - sc1
        can't be a boot volume, lowest cost is important, infrequently accessed, archive

Understand Pre-Warming EBS Volumes
    reading from all blocks before use
    now only needed if restored from a snapshot

CloudWatch Metrics
    VolumeReadBytes
    VolumeWriteBytes
    VolumeReadOps
    VolumeWriteOps
    VolumeTotalReadTime
    VolumeTotalWriteTime
    VolumeIdleTime
    VolumeQueueLength - outstanding requests
    VolumeThroughputPercentage - provisioned IOPS volumes only
    VolumeConsumedReadWriteOps - provisioned IOPS volumes only

Volume Status Checks
    ok
    warning
    impaired
    insufficient-data

If an Amazon EBS volume is attached to a current gen EC2 instance type, you can increate its sieze, change its volume type, or adjust its IOPS perforance all without detaching the volume.  <-- will likely not be on the exam as it is too new>

