## Introduction
Usually when applications (projects) are deployed in a cluster or multiple clusters, its normal to have a Prometheus server 
to monitor application specific metrics. The clusters also will have their own Prometheus to monitor cluster wide metrics.

Once Prometheus servers are scaled out horizontally based on any strategy of sharding, Prometheus federation is often needed 
to have an overall monitoring view for aggregating some of the metrics. 


![Scaling Prometheus](https://github.com/nrchakradhar/Notes/blob/master/PrometheusFederation/images/Prometheus_Scaling.png)


### Prometheus supports two types of federation
* Hierarchical
* Cross service
depicted in the following diagram.

![Types of Federation](https://github.com/nrchakradhar/Notes/blob/master/PrometheusFederation/images/Prometheus_Federation.png)

## What is not so good about Federation
Federation should be used to pull in a limited set of metrics OR a limited set of aggregated time series from other Prometheus server.
Federation is bad when large sets of time series is being replicated. The problems are to do with performance, scaling, reliability.
Dimensioning, alerting and correctness of data has to be kept in mind when doing federation.

## References
https://prometheus.io/docs/prometheus/latest/federation/

https://www.robustperception.io/federation-what-is-it-good-for

https://stackoverflow.com/questions/48751632/prometheus-federation-match-params-do-not-work

Images are from Google Search. Missed the link. Will update once I find it.
