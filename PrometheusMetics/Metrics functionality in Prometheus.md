## Introduction
Prometheus is the most widely used observability tool in all cloud or non-cloud deployments. When somebody says they are using Prometheus, we need to ask 
the specific question about what exact functionality offered by Prometheus they are using. The need for this is due to the different use cases for which
and its eco-system has been used.

## Reference
An excellent [blog by Julius Volz](https://promlabs.com/blog/2020/10/13/the-meaning-of-prometheus) clearly articulates the same.

For a use case that only wants to have metrics scraped from targets and shipped to a chosen backend storage, a limited functionality of Prometheus would be sufficient.
This might appear to be moving away from pull model that Prometheus articulates, but it need to be viewed so. The interfaces developed by Prometheus has gained wide
acceptance and hence newer possibilities around the interface is possible. I would like to understand the interface for metrics collection, remote write and query 
based on PromQL.

## TO DO
Add a diagram showing what is mentioned above
Give snippets of each interface and references to interface standard
