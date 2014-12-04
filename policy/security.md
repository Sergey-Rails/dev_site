---
layout: page
section: policy
title: Security
permalink: /security/
---

The Spree community takes security issues very seriously. The open source nature of the software makes it possible for anyone to review the source code and perform their own security audit. If you believe you have found a potential security vulnerability in the software please report the issue by sending a private email to [security@spreecommerce.com](mailto:security@spreecommerce.com).

### Disclosure

Please do not announce or discuss potential security vulnerabilities in public. We are greatful for the assistance of whitehat security researchers and we will make sure that you and/or your organization get full public credit once we publicly disclose the issue (along with the fix). We promise to work quickly to determine the severity of the issue and work with you to help provide a fix for any affected versions of our software.

### Providing a Security Patch

If you would like to provide a patch for the security issue please do not open a pull request for it. Please create a commit on your own private copy of Spree and run this command:

```
$ git format-patch HEAD~1..HEAD --stdout > patch.txt
```

This command will generate a file named 'patch.txt' with your changes. Please email a description of the patch along with the patch itself to [security@spreecommerce.com](mailto:security@spreecommerce.com).

### Bounties

Spree is an open source project supported by volunteers.  Unfortunately we do not currently have a budget to pay bounties to security researchers.  We are currently looking into the possibility of getting some private donations to support such a fund.