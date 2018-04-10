ELB is monitored every 60 seconds (provided there is traffic)

ELB Metrics
    HealthyHostCount
    UnHealthyHostCount
    RequestCount
    Latency
    HTTPCode_ELB_4XX
    HTTPCode_ELB_5XX
    HTTPCode_Backend_2XX
    HTTPCode_Backend_3XX
    HTTPCode_Backend_4XX
    HTTPCode_Backend_5XX
    BackendConnectionErrors
    SurgeQueueLength - pay attentions to this, pending requests, can build auto-scaling groups from this metric
    SpilloverCount - pay attention to this, rejected requests due to queue being full
    