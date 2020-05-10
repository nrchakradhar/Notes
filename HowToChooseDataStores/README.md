# How to choose data stores.
There are a variety of data stores available in open source as well as from different cloud vendors. 
The landscape is quite huge and it can be a case of spoilt for choices.

## How to pick a data store?
Before we decide a data store for usage, we need to find the answer for the question
* What is the type of data with which we plan to deal in terms of storage and computation?
* What are the non functional requirements

We may look at use-cases that we are planning to handle. Based on the use-case, the nature of data can also be derived. 
Also based on the type of application we plan to build, the nature of data can be determined.

[CNCF SIG Storage whitepaper](https://github.com/cncf/sig-storage/blob/master/CNCF%20Storage%20Landscape%20-%20White%20Paper.pdf) outlines the different characteristics of data and associated computation stack. Based on the needs and choices made a particular data store can be picked. If a specific one is not available, then one has to be created :star: :smile:


For more details you can refer to Azure and AWS guides.

[Azure](https://docs.microsoft.com/en-us/azure/architecture/guide/technology-choices/data-store-comparison)
The article has information about different data requirements one may have and different non functional requirements.

AWS [Databases](https://aws.amazon.com/products/databases/) and [Analytics](https://aws.amazon.com/big-data/datalakes-and-analytics/) 
view the choices from use cases perspective.

## Conclusion
For addressing a set of business use cases, there will not be a a one-size fits all solution that we may find. We have to mix-match and adapt the different solutions available.

The following link is useful to get a high level view of E2E analytics pipelines.
https://towardsdatascience.com/scalable-efficient-big-data-analytics-machine-learning-pipeline-architecture-on-cloud-4d59efc092b5
