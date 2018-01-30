+++
# Date this page was created.
date = "2018-01-30"

# Project title.
title = "Contracts Federated Cloud"

# Project summary to display on homepage.
summary = "A Contracts-based Federated Cloud Architecture"

# Optional image to display on homepage (relative to `static/img/` folder).
image_preview = "Intro-Contracts.png"

# Tags: can be used for filtering projects.
# Example: `tags = ["machine-learning", "deep-learning"]`
tags = ["cloud", "game-theory"]

# Optional external URL for project (replaces project detail page).
external_link = ""

# Does the project detail page use math formatting?
math = false

# Optional featured image (relative to `static/img/` folder).
[header]
image = ""
caption = ""

+++
# Overview


We develop a new contracts-based resource sharing model for federated geo-distributed clouds that allows cloud service providers to establish contractual relationships with individual datacenters for defined time intervals. Based on the established contracts, individual cloud service providers employ a cost-aware job scheduling and provisioning algorithm that enables tasks to complete and meet their response time requirements. 

## What is the challenge? 
 + How to decide Resource Sharing Contracts guaranteeing both Fairness and Efficiency?
 + How to quantify utility of the contracts for the Cloud Service Providers?
 + How to Schedule Jobs in a contracts-aware manner among the available Geo-distributed Data Centers?

## How the System Works?
 + Auction-based Contracts Establishment (Designed based on McAfee Mechanism)
    + Truthfulness: No incentives to Cheat Makes the Market More Efficient and Fair
    + Budget Balance: Keeps the Resource Allocation process Sustainable 
    + Naturally Finds the Equilibrium Between Supply and Demand
 + Fine-grained Utility Function Design considering:
    + Operating Cost
    + Payment from Users
    + Penalty for Violating SLAs
 + Resource Sharing Contracts
    + Relatively Long Contracts Avoid Frequent Migrations
    + Predetermined Allocations minimize Disruption of Normal Operations in the Data Centers
 + Cost-aware Scheduling 
    + Optimize the Cost of Using Contracts

**Publications**

 + Jinlai Xu, Balaji Palanisamy (2017). [Cost-aware Resource Management for Federated Clouds Using Resource Sharing Contracts](https://www.researchgate.net/publication/317097662_Cost-Aware_Resource_Management_for_Federated_Clouds_Using_Resource_Sharing_Contracts), IEEE Cloud 2017.
 + Jinlai Xu, Balaji Palanisamy (2018). [Optimized Contract-based Model for Resource Allocation in Federated Geo-distributed Clouds](https://www.researchgate.net/publication/322691834_Optimized_Contract-based_Model_for_Resource_Allocation_in_Federated_Geo-distributed_Clouds), IEEE TSC.
 
**Slides**

<iframe src="https://onedrive.live.com/embed?cid=E1DD6EDD2DA4DFBE&resid=E1DD6EDD2DA4DFBE%2121398&authkey=ANCwepdLkgdg-Xo&em=2" width="600" height="450" frameborder="0" scrolling="no"></iframe>
