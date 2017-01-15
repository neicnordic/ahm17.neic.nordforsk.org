---
organizers: Gurvinder Singh
title: "Intro to Kubernetes and hands-on for deploying a Jupyter Notebook"
---

This tutorial will provide brief introduction to
[Kubernetes](http://kubernetes.io) concepts and its architecture. Participants
will later deploy a Jupyter Notebook application on Kubernetes running on their
laptop first and then the same application on Kubernetes cluster in the cloud.
They will also see how we can automate DNS, SSL certs too when deploying
application on Kubernetes. The list of required software to be pre-installed on
your laptop will be provided before the workshop.

Basic understanding of containers ([Docker](https://www.docker.com)) can be
helpful for this tutorial. The participants need to have Linux or Mac OS X
running on their laptop, as we are not going to support windows during hands
on.

Please install the following four tools **before** the tutorial:

- Git
- Virtualbox
- Kubernetes client
- Minikube

For Git and Virtualbox, we recommend to install using usual package
installation tools or their corresponding webpages.


#### Kubernetes client

Get the kubectl client to deploy application on kubernetes cluster.

For MAC OSX (amd64):

```shell
$ wget -qO - https://storage.googleapis.com/kubernetes-release/release/v1.5.1/kubernetes-client-darwin-amd64.tar.gz | tar zxf - && sudo mv kubernetes/client/bin/kubectl /usr/local/bin
```

For Linux (amd64):

```shell
$ wget -qO - https://storage.googleapis.com/kubernetes-release/release/v1.5.1/kubernetes-client-linux-amd64.tar.gz | tar zxf - && sudo mv kubernetes/client/bin/kubectl /usr/local/bin
```

Make sure you are able to run:

```shell
$ kubectl help
```


#### Minikube Setup

Make sure your Virtualbox setup is working before starting with Minikube.
Install the Minikube to have a local Kubernetes cluster.

For MAC OSX (amd64):

```shell
$ curl -Lo minikube https://storage.googleapis.com/minikube/releases/v0.14.0/minikube-darwin-amd64 && chmod +x minikube && sudo mv minikube /usr/local/bin/
```

For Linux (amd64):

```shell
$ curl -Lo minikube https://storage.googleapis.com/minikube/releases/v0.14.0/minikube-linux-amd64 && chmod +x minikube && sudo mv minikube /usr/local/bin/
```

Now verify that you are able to run:

```shell
$ minikube help
```

To avoid network congestion during tutorial, run these commands to download iso images and other dependencies:

```shell
$ minikube start  # this step can take some time
$ minikube stop
```
