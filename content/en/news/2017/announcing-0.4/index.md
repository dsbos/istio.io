---
title: Announcing Istio 0.4
description: Istio 0.4 announcement.
publishdate: 2017-12-18
attribution: The Istio Team
release: 0.3
aliases:
    - /about/notes/older/0.4
    - /docs/welcome/notes/0.4.html
    - /about/notes/0.4/index.html
---

This release has only got a few weeks' worth of changes, as we stabilize our monthly release process.
In addition to the usual pile of bug fixes and performance improvements, this release includes the items
below.

{{< relnote >}}

## General

- **Cloud Foundry**. Added minimum Pilot support for the [Cloud Foundry](https://www.cloudfoundry.org) platform, making it
possible for Pilot to discover CF services and service instances.

- **Circonus**. Mixer now includes an adapter for the [Circonus](https://www.circonus.com) analytics and monitoring platform.

- **Pilot Metrics**. Pilot now collects metrics for diagnostics.

- **Helm Charts**. We now provide Helm charts to install Istio.

- **Enhanced Attribute Expressions**. Mixer's expression language gained a few new functions
to make it easier to write policy rules. [Learn more](/docs/reference/config/policy-and-telemetry/expression-language/)

If you're into the nitty-gritty details, you can see our more detailed low-level
release notes [here](https://github.com/istio/istio/wiki/v0.4.0).
