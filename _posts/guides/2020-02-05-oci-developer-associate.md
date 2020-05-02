---
layout: post
title: Oracle Cloud Infrastructure (OCI) Developer Associate exam2020 (1Z0-1084) guide (dz-s)
categories: [guides]
tags: [certification, oci, exam]
---


This series of articles is aimed to describe my own path of preparation to OCI-* sertification exams. Despite Oracle provides set of videos to prepare, i decided to create these articles to combine all information by topics in a readable format (i don't really like videos as a source for studying).

## Exam Topics

1. Cloud Native Fundamentals
    1. [Describe Cloud-Native Building Blocks](#describe-cloud-native-building-blocks)
    2. Understand the Service Communication Patterns
    3. Role of Protocols and their benefits in
    communication pattern
  
2. Developing Cloud Native Applications
    1. Developing Serverless Application with Oracle Functions
    2. Developing Microservices and applications for OKE
    3. Using Data in Cloud Native
    4. Using OCI APIs, SDKs and CLI
3. Securing Cloud Native Applications
    1. Security challenges with Cloud Native
    2. Defense-in-depth approach
    3. Configuration and Secret Management
    4. Using IAM for authn/authz
4. Testing Cloud Native Applications
    1. Challenges of testing in Cloud Native world
    2. Managing multiple environments (dev, test/stage, prod)
5. Operating Cloud Native Applications
    1. Managing Infrastructure
    2. Building, deploying and releasing applications
    3. Monitoring, observability, and alerting 

So, let's begin.

# Describe Cloud-Native Building Blocks

It will be based on Oracle Official guide [Become OCI Developer (Associate)](https://learn.oracle.com/ols/learning-path/become-oci-developer-associate/35644/75248), but i will try to broaden this information with additional sources to make this guide less specified for understanding 

So, in the beginning of Oracle's course we are describing common pronciples of building and support distributed system.
First of all we are introduced with two common approaches:

Pets :cat:
 - Treat you infrastructure like pets
 - Give them names, IP adresses, care of them, keep them updated.

Cattels :cow: 
 - Everything is a number
 - No attachment
 - If something goes wrong, you replace it

Here, i'm not quite sure what we can detalize, i would suggest to look at implementations of these strategies on practice at the end of 1st item.

**Patterns for building cloud-native applications**

Cloud Native vs Traditional Arch:

**Stateful vs. Stateless**
 - State stored with the compute instance
 - Load balancers using sticky sessions
 - What happens on reboot or cash

**Service orchestration vs. Service choreography**
 - Multiple services orchestrated to work as one, using sync communication
 - Choreography uses eventing system

**Dealing with failures**
 - Minimize failures vs. expect and deal with them

Quite common words, then we have CAD theorem pic:

<!-- .element height="50%" width="50%" -->
<img src="/assets/CAD.png" width="100%">

Next slide is about Microservices / Containers + Functions.

**Microservices** &ndash; architechture

**Containers + Functions** &ndash; services, elements of our arch.