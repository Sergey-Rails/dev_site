---
layout: page
section: policy
title: New Features
permalink: /new_features/
---

Spree is currently being used to power over 50,000 storefronts. The open source nature of our project allows to take advantage of continuous feedback and innovation. It is also important, however, that we follow a disciplined set of rules in order to ensure stability.

## Bug Fix vs. Feature

We have policies for how we treat bugs and new features. It's important to understand how we define both of those terms so we'll do so here now.

#### Bug Fix

A bug fix is best defined as an internal change that fixes incorrect behavior. Bug fixes do not add or subtract new elements or text to the UI. Style changes in a bug fix are limited to correcting an obvious visual flaw in how something is rendered on a particular device.

<span class="warning">It's not a bug just because you don't like the way a feature currently behaves or looks.</span>

Performance improvements and code refactoring are not considered bug fixes - even if they do not change or break the public API. We're always open to improvements but those improvements (even minor ones) will be classified as features when it comes to how we handle them.

#### Feature

A feature is any change to the code that does not fall under the definition of a bug fix. Period. We welcome all types of feature contributions, big or small as well as enhancements to existing features. They will all be treated the same, however, when it comes to our [release policy](/releases).

## Pull Requests

New features must always added through a [pull request](/pull_requests). This accomplishes two objectives. The first is that it provides transparency and an opportunity for public debate. The second is that it ensures that we maintain a high quality of code since all pull requests are carefully vetted before they are merged.

#### All Tests Must Pass

All pull requests are automatically run against our [full test suite](https://circleci.com/gh/spree/spree). Github will provide an indication of whether or not the tests are passing and let you know it's safe to merge.

![All tests passing](/assets/passing_test_suite.png)

#### No Style Violations

All code changes should be consistent with our [code style policy](/code_style). We use [Hound CI](https://houndci.com/) to flag any issues which violate our guidelines. Violations will be identified in the PR comments.  All violations must be fixed before the PR is merged.

![Style problem](/assets/hound_ci.png)

_The automated rules used to enforce our code style are still a work in progress. We are tweaking as necessary whenever we identify an unreasonable (or false positive)._

#### Core Team Signoff

All new features (or changes to existing features) must be signed off by at least three members of the core team. Signoff is done by core team members adding a "+1 signoff" comment to the pull request. If the feature is being proposed by a member of the core team this still requires an additional three "+1" votes.

Members of the community will often use "+1" as shorthand for "I'm generally in favor". These expressions of support, whether they are from core team members or otherwise, do not constitute a signoff. The core team member must include the "signoff" in their comment and should only do so after personally testing and reviewing the functionality.