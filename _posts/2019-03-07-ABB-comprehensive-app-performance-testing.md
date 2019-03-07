---
layout: post-sidebar
date: 2019-03-07
title: "Architecture Building Block: Comprehensive Performance Testing"
categories: technology
author_name : Kris Bravo
author_url : /author/kris
author_avatar: kris
show_avatar : true
read_time : 15
feature_image: feature-water
show_related_posts: true
square_related: recommend-spain
---

It is a wonderful feeling to come up with an idea, take the risks to make it real, and be rewarded with customers.  Even more so when you need to serve an increasingly large number of users.

Once you are up and running it is important to keep the promise to help your customers when there are more of them. Some of the issues that undermine that promise come from performance issues during high traffic volume.

I found an article from SmartBear about the topic that was interesting. It describes the types of performance testing you can use, and what their purpose is. Here is a link to the article:

[Smartbear: 7 Types of Web Performance Tests and How They Fit Into Your Testing Cycle](https://smartbear.com/blog/test-and-monitor/7-types-of-web-performance-tests-and-how-they-fit/)

Beginning with this article I created the following reference architecture. You can see how the various test types fit together. Pay attention to the important parts like duration, scheduling, and deployment phase where tests are executed. A good plan will make it easy to recall the important metrics - functional coverage %, certified load volume, and concurrent user limit.

# Types of Performance Tests

The seven types of tests applied are as follows:

* Smoke Tests
* Load Tests
* Performance Tests
* Capacity Tests
* Stress Tests
* Component Tests
* Soak Tests

Each test is used to achieve a goal of the Product Testing Process. A testing platform is used to execute the tests and report on whether the goals are met by the product release version you are testing.

# Product Testing Process

Simply put, this process is that of a Product Tester executing tests using one or more services and following a plan. There are other tests conducted earlier in the product delivery lifecycle; but for performance the goals are easily stated:

* Confirm all features are working
* Prevent old defects from returning
* Establish the ratio of resources required to transactions processed
* Define the TPS rate the system can handle
* Confirm that the system responds according to requirements
* Spot changes in the ability to process transactions since the last version
* Establish a basis for setting alerts and monitoring thresholds
* Identify the component that will fail first when load exceeds capacity
* Validate the performance of a specific component 
* Identify memory leaks

# Spotting Smoke and Turning up the Heat

The core of the entire performance test approach is a feature complete set of tests. Running these each time the product is changed will help spot new problems and regressions that can be addressed before significant time and resources are committed to further testing.

This initial smoke test suite is then re-used at increasily higher volumes and for longer periods of time to target the other goals. Once the system slows down or fails to respond at all the suspect components can be improved or replaced.

# Tailoring the Testing

Use your application architecture to identify a testing service or services. Start with a plan with clear goals and specific kinds of testing. Set parameters for how long and at what volumes tests will run. Be sensible about those values - there is no sense in running a long performance test when a soak test is planned for that evening.

The product that you have after the testing is complete and the issues are addressed will then be a promise kept.



![Comprehensive Performance Testing Reference ArchitectureMinikube Features]({{site.url}}/{{site.baseurl}}img/post-assets/2019-03-07_ABB-cpta.png)


