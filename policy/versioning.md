---
layout: page
section: policy
title: Versioning
permalink: /versioning/
---

Starting with the Spree 3.0 release, we will be following a policy of [Semantic Versioning](http://semver.org/). The public API for this release will be defined as the REST API. The public API for Spree 3.0 will consist of all public methods.  The Spree 4.0 release will contain a fully documented public API (with rdoc) for all classes and methods (in addition to a REST API).

### Major Version

Major version X (X.y.z) must be incremented if any backwards incompatible changes are introduced to the public API. It may include minor and patch level changes. Patch and minor version must be reset to 0 whenever the major version is incremented.

### Minor Version

Minor version Y (x.Y.z) must be incremented if new, backwards compatible functionality is introduced to the public API. It must be incremented if any public API functionality is marked as deprecated. It may be incremented if substantial new functionality or improvements are introduced within the private code. It may include patch level changes. Patch version must be reset to 0 whenever the minor version is incremented. An update to a gem dependency (ex. Rails) would constitute a minor version increase unless that change causes the public API to break (in which case the major version is incremented instead).

### Patch Version

Patch version Z (x.y.Z) must be incremented if only backwards compatible bug fixes are introduced. A bug fix is defined as an internal change that fixes incorrect behavior. Security fixes can also be done as a patch version provided they are fully backwards compatibile and do not introduce new functionality.