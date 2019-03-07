---
layout: post-sidebar
date: 2019-03-07
title: "Architecture Building Block: Comprehensive Performance Testing"
categories: technology
author_name : Kris Bravo
author_url : /author/kris
author_avatar: kris
show_avatar : true
read_time : 30
feature_image: feature-water
show_related_posts: true
square_related: recommend-spain
---

It is a wonderful feeling to come up with an idea, take the risks to make it real, and be rewarded with customers.  Even more so when you need to serve an increasingly large number of users.

Once you are up and running it is important to keep the promise to help your customers when there are more of them. Some of the issues that undermine that promise come from performance issues during high traffic volume.

I found an article from SmartBear about the topic that was interesting. It describes the types of performance testing you can use, and what their purpose is. Here is a link to the article:

[Smartbear: 7 Types of Web Performance Tests and How They Fit Into Your Testing Cycle](https://smartbear.com/blog/test-and-monitor/7-types-of-web-performance-tests-and-how-they-fit/)

Beginning with this article I created the following reference architecture. You can see how the various test types fit together. Pay attention to the important parts like duration, scheduling, and deployment phase where tests are executed. A good plan will make it easy to recall the important metrics - functional coverage %, certified load volume, and concurrent user limit.

![Comprehensive Performance Testing Reference ArchitectureMinikube Features]({{site.url}}/{{site.baseurl}}img/post-assets/2019-03-07_ABB-cpta.png)


