---
layout: post
title:  "Architecture Building Block: Kubernetes Container Management"
date: 2018-12-05 08:50:28
categories: technology
author_name : Kris Bravo
author_url : /author/kris
author_avatar: kris
show_avatar : true
read_time : 15
feature_image: feature-wolf
show_related_posts: false
square_related: recommend-wolf
---

If you are thinking about adding Kubernetes to your architecture it's nice to have a starting point that shows what all is included and how they fit together.

![Fire image]({{site.url}}/{{site.baseurl}}img/post-assets/2018-12-05_ABB-kcm.png)

You're basically looking at two node types - master and worker - with network interactions between an API and runtime service.

# Master Node

Okay, arguably the terminology is falling out of favor, and should be. The master, or management node is responsible for services that are required to orchestrate the activity across all nodes.

## Master Service

This service contains the schedule and controller manager, and serves up an API interface for interacting with the worker nodes.

## etcd Service

Configuration management is provided by an etcd service.

# Worker Node

The worker node operates two services. This node scales out according to the requireed number of containers and their required resources.

## Workload Service

The workload service contains a user pod component that runs the actual Docker containers.

## Kubelet Service

The Kubelet Service is the agent working on behalf of the management node to ensure that the specified number of containers are running and healthy.

![Minikube Features]({{site.url}}/{{site.baseurl}}img/post-assets/2018-12-05_ABB-kf.png)

Here is a list of features provided by Kubernetes. If you run minikube there are commands and flags to become familiar with.

[Kubernetes](https://kubernetes.io)

[Minikube](https://kubernetes.io/docs/setup/minikube/)

[8 Steps to Becoming Awesome with Kubernetes](http://bit.ly/8stepsawesome)

[Archimate Model]({{site.url}}/{{site.baseurl}}bravok.github.io.archimate)
