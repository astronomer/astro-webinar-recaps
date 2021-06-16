---
slug: official-airflow-helm-chart
title: Getting Started With the Official Airflow Helm Chart
description: The official helm chart of Apache Airflow is out! The days of wondering what Helm Chart to use in production are over.
heroImagePath: ../assets/airflowHelmChartMeta.png
authors:
  - Brandon Medina
date: 2021-06-15T00:00:00.000Z
---

<iframe src="https://fast.wistia.net/embed/iframe/gviwd9gp2c" title="Dynamic Dags Video" allow="autoplay; fullscreen" allowtransparency="true" frameborder="0" scrolling="no" class="wistia_embed" name="wistia_embed" allowfullscreen msallowfullscreen width="100%" height="450"></iframe>

The official helm chart of Apache Airflow is out! The days of wondering what Helm Chart to use in production are over.

Now you can safely deploy Airflow in the production environment using an official chart maintained and tested by Airflow PMC members as well as the community.

**Why is this great news?**

* If Airflow gets updated, so does your Helm Chart
* You can quickly run some experiments with new features of Airflow, for example KEDA
* You can easily run local experiments

At the end of the webinar, you will have a fully functional Airflow instance deployed with the Official Helm Chart and running within a Kubernetes cluster locally.

In this webinar we’ll show you how to:
* Create a Kubernetes cluster with KinD in local
* Deploy Airflow in a few seconds with the Official Helm Chart
* Discover the first parameters to configure in the Helm Chart
* Synchronize your DAGs with a Git repository
* (BONUS!) Get your task’s logs

## Step 1: Create the local Kubernetes cluster

> Note: *you need to have Docker, Docker Composer, kubectl, and Kind installed.*

1. Open the `kind-cluster.yaml` file — here you define your cluster. 

You can see here different `worker` nodes. Each worker node you can configure and specify.

![airflow-helm-chart-.png](../assets/airflow-helm-chart-.png)

2. Type the command `kind create cluster --name airflow-cluster --config kind-cluster.yaml`

![airflow-helm-chart-.png](../assets/airflow-helm-chart-.png)

