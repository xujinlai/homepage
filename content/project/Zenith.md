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
tags = ["edge", "game-theory"]

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

In the Internet of Things(IoT) era, the demands for low-latency computing for time-sensitive applications (e.g., location-based augmented reality games, real-time smart grid management, real-time navigation using wearables) has been growing rapidly. Edge Computing provides an additional layer of infrastructure to fill latency gaps between IoT devices and the backend computing infrastructure.

*Zenith* decouples **resource allocation** and **service provisioning and management** at the edge and provides a novel model to allocate resources at the edge to maximize utility. Zenith aims at increasing the overall resource allocation efficiency by allowing resources to be allocated and shared in a latency-aware manner. 

## What is the challenge? 
 + Fair and Efficient Resource Allocation across Geographically Distributed Edge Resources
 + Fast Service Discovery on Highly Distributed Micro Data Centers

## How Zenith Works?
 + Geographic Division usingWeighted Vonoroi Diagram (WVD)
    + Service Discovery with Constant Time
    + Naturally Satisfies Latency-Sensitive Workloads with Nearest Service Discovery
    + Dynamically Balances the Workloads Between Micro Data Centers
    + Easy and Fast to Update
 + Auction-based Resource Allocation
    + Truthfulness: No Incentives for Cheating. 
    + Budget Balance: Keeps the Allocation Process more Sustainable
    + Naturally Finds the Equilibrium Between Supply and Demand
 + Resource Sharing Contracts
    + Longer duration of Contracts Avoid Frequent Migrations
    + Stable Running Environment Suits the Requirements for Latency-Sensitive Workloads

**Publications**

 + Jinlai Xu, Balaji Palanisamy, Heiko Ludwig, Qingyang Wang (2017). [Zenith: Utility-aware Resource Allocation for Edge Computing](https://www.researchgate.net/publication/317097920_Zenith_Utility-aware_Resource_Allocation_for_Edge_Computing), IEEE Edge 2017.
 
**Slides**

<iframe src="https://onedrive.live.com/embed?cid=E1DD6EDD2DA4DFBE&resid=E1DD6EDD2DA4DFBE%2121505&authkey=AK5qp4kx3NvYRag&em=2" width="600" height="450" frameborder="0" scrolling="no"></iframe>