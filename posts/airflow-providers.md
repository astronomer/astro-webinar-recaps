---
slug: airflow-providers
title: Webinar Recap - Airflow Providers
description: Learn everything about Airflow 2.0 providers including what defines a provider, how to create your own provider, and customizing provider packages.
heroImagePath: ../assets/providersMeta.png
authors:
  - Eric Griffing
  - Brandon Medina
date: 2021-04-06T20:23:50.045Z
---

<!-- markdownlint-disable MD033 -->
<iframe src="https://fast.wistia.net/embed/iframe/brvfkmikra" title="[Webinar Recap] Airflow 2.0 Providers Video" allow="autoplay; fullscreen" allowtransparency="true" frameborder="0" scrolling="no" class="wistia_embed" name="wistia_embed" allowfullscreen msallowfullscreen width="100%" height="450"></iframe>

## Airflow Provider Framework

Providers are Python packages containing all relevant modules for a specific service provider (ie. AWS, Snowflake, Google etc.)

Unlike Apache Airflow 1.10, now [Airflow 2.0](https://www.astronomer.io/blog/introducing-airflow-2-0) is delivered in multiple, separate but connected packages. The core of the Airflow scheduling system is delivered as `apache-airflow` package and there are around [60 Airflow Provider Packages ](https://registry.astronomer.io/)which can be installed separately.

In Airflow 2.0, Providers are decoupled from core Airflow releases: 

* Providers can now be independently versioned, maintained, and released
* Users just \`pip install\` the provider package and then import modules into their DAG files
* Providers can now be built from any public repository 



## The Astronomer Registry

![Astronomer Registry](../assets/providers-1.png)

Recently we announced [The Astronomer Registry](http://registry.astronomer.io/): a discovery hub for Airflow providers designed to bridge the gap between the Airflow community and the broader data ecosystem.

The [Airflow providers framework](http://airflow.apache.org/docs/apache-airflow-providers/) has long been a valuable asset for the community. DAG authors benefit from access to a deep library of standard patterns while maintaining code-driven customizability; it enables a tight integration between Airflow and almost any tool in the modern data stack.

The easiest way to get started with providers and Apache Airflow 2.0 is by using the Astronomer CLI. To make it easy you can get up and running with Airflow by following our [Quickstart Guide](https://www.astronomer.io/guides/get-started-airflow-2).
