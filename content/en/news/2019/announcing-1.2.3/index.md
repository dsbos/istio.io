---
title: Announcing Istio 1.2.3
description: Istio 1.2.3 patch release.
publishdate: 2019-08-02
attribution: The Istio Team
release: 1.2.3
aliases:
    - /about/notes/1.2.3
    - /blog/2019/announcing-1.2.3
---

We're pleased to announce the availability of Istio 1.2.3. Please see below for what's changed.

{{< relnote >}}

## Bug fixes

- Fix a bug where the sidecar could infinitely forward requests to itself when pod defines a port undefined for service ([Issue 14443](https://github.com/istio/istio/issues/14443)) and ([Issue 14242](https://github.com/istio/istio/issues/14242))
- Fix a bug where Stackdriver adapter shuts down after telemetry is started.
- Fix Redis connectivity issues.
- Fix case-sensitivity in regex-based HTTP URI matching for Virtual Service ([Issue 14983](https://github.com/istio/istio/issues/14983))
- Fix HPA and CPU settings for demo profile ([Issue 15338](https://github.com/istio/istio/issues/15338))
- Relax Keep-Alive enforcement policy to avoid dropping connections under load ([Issue 15088](https://github.com/istio/istio/issues/15088))
- When SDS is not used, skip Kubernetes JWT authentication to mitigate the risk of compromised (untrustworthy) JWTs being used.

## Tests upgrade

- Update base image version for Bookinfo reviews sample app ([Issue 15477](https://github.com/istio/istio/issues/15477))
- Bookinfo samples image qualification ([Issue 14237](https://github.com/istio/istio/issues/14237))
