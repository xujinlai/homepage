+++
# Date this page was created.
date = "2017-05-24"

# Project title.
title = "Zenith"

# Project summary to display on homepage.
summary = "An Innovation on Edge Computing Architecture"

# Optional image to display on homepage (relative to `static/img/` folder).
image_preview = "Zenith-Intro.png"

# Tags: can be used for filtering projects.
# Example: `tags = ["machine-learning", "deep-learning"]`
tags = ["edge"]

# Optional external URL for project (replaces project detail page).
external_link = ""

# Does the project detail page use math formatting?
math = false

# Optional featured image (relative to `static/img/` folder).
[header]
image = "headers/Zenith-Intro - banner.png"
caption = "Proposed Decoupled Edge Computing Architecture: *Zenith* :smile:"

+++

## Overview

*Zenith* is a project for achieving efficient resource allocation and usage for Fog/Edge Computing. As the explosion of IoT, the Cloud Computing model is not enough for supporting latency-sensitive applications for massive amount of IoT devices. 
Fog/Edge Computing is emerging to fill the gap between the Cloud and the end-points. 

*Zenith* decouples the **Resource Allocation** and **Service Provisioning and Management** at the edge, which provides a novel model to allocate the resources at the edge to both maximize the utility of the service providers and the profits of the edge infrastructure providers. This model also increase the overall efficiency by allowing all the resources to be shared with the service providers which is represented in the simulations. 

## What is the challenge? 
 + Fair Resource Allocation between Multiple Service Providers
 + Fast Service Discovery on Massive Micro Data Centers

## How Zenith Works?
 + Region Division by Weighted Vonoroi Diagram (WVD)
    + Service Discovery with Constant Time
    + Natually Satisfies the Sensitive Latency Workloads
    + Dynamically Balance the Workloads Between the Micro Data Centers with Ajusting the Weights for each Micro Data Centers
    + Easy and Fast to Update
 + Auction-based Resource Allocation
    + Truthfulness: No Intuitive to Cheat Makes the Market with More Fairness
    + Budget Balance: Keeps the Federation with Sustainable Development
    + Naturally Finds the Equilibrium Between the Supply and Demand
 + Resource Sharing Contracts
    + Relative Long Time Contracts Avoid Frequently Migration
    + Stable Running Environment Suits the Requirements for Latency-Sensitive Workloads

**Publications**

 + Jinlai Xu, Balaji Palanisamy, Heiko Ludwig, Qingyang Wang (2017). [Zenith: Utility-aware Resource Allocation for Edge Computing](https://www.researchgate.net/publication/317097920_Zenith_Utility-aware_Resource_Allocation_for_Edge_Computing), IEEE Edge 2017.