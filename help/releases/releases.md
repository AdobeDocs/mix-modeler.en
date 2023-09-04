---
description: Explains the continuous feature release strategy for Adobe Mix Modeler
title: Adobe Mix Modeler releases
feature: Release Notes
---
# Adobe Mix Modeler releases

Adobe Mix Modeler releases operate on a continuous delivery model which allows for a scalable, phased approach to feature deployment.


## Release strategy

Adobe Mix Modeler uses feature flags (also known as "toggles") to control the visibility of new features, allowing for controlled scale testing prior to full release. This release strategy includes the following phases:

* **Limited Testing**: A phased release begins with testing by internal Adobe users. It is then made available to a small group of customer accounts to ensure that the feature meets customer needs and expectations. 

* **Start of Rollout**: Rollout of a phased release begins with the Limited Testing phase. The release is then scaled from 0% to 100% availability to customers over the course of a couple months. Phased rollout happens at the Experience Cloud Organization level, so all entitled users in an organization receive the same experience.

* **General Availability (GA)**: The feature is available to 100% of entitled Experience Cloud organizations, and feature release is complete.

With each feature release, the timeline from release start to general availability may vary. The goal is to keep releases short, so that within 2 months of release start, a feature will be generally available.


## Feature flags

Feature flags are used to control the visibility of new features during release. Adobe recommends adding `app.launchdarkly.com` to your firewall's [allowed list](https://experienceleague.adobe.com/docs/analytics/technotes/ip-addresses.html) for an optimal experience during release. Shortly after general availability is reached, the flag is removed.


## Benefits

Phased releases enable Adobe to better scale the software deployment process and ensure features are fully hardened before general availability. It also allows features to be released as soon as they are available, rather than adhering to a fixed monthly release window.

## FAQs

| Question | Answer |
| --- | --- |
| Can I request early access to a feature? | No. Early access will not be granted. |
| Does this release strategy affect my access to features? | No. Once a feature has reached general availability, you will have access to the feature if it is included in your Adobe Mix Modeler license. |