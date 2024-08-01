---
description: For clients who want the best
---

# Standard deployments

### Brief

Standard deployments are fully managed deployments that rely on leading cloud vendors. The Hamanahel suite in standard deployment is primarily a multi-vendor deployment that optimizes costs by selecting key services from vendors that work well with our suite while also preventing vendor lock-in.

### Regions

Standard deployments are region-bound and often default to where Amazon Web Services has a region. While we opt to utilize multiple vendors, we try to work around AWS's regions since most of our suite is built to leverage AWS's cost-saving tools. Considering the broad availability of regions with AWS, we've not had to deploy in a region without an AWS region, yet. Currently, Standard deployments are available without additional charges in Mumbai and Sydney.\


1. Mumbai \[ap-south-1]
2. Sydney \[ap-southeast-1]
3. UAE \[me-central-1] \*[^1]
4. North Virginia \[us-east-1] \*[^2]

### Service Outline

The deployment primarily relies on deploying load-balanced clusters of application servers, databases, and complementary services such as cache servers, email services, queues, etc. The deployment focuses on being highly available and hence relies on managed services from vendors. Each tenant in our service is provisioned with dedicated tenancy resources to establish security and reliability.

### Backups

We provide up to 30 days of point-in-time restoration of data. This duration can be increased for a fee.

### Notes on Azure

Hamanahel in the past has used Azure as a primary vendor and continues to support Azure managed services suite. However long terms prospects in commitment-based cost-savings had us transition to AWS. We do however still support and encourage Enterprise deployments to Azure regions.\
\
\


[^1]: Provisional deployment

[^2]: Provisional deployment
