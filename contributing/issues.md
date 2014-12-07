---
layout: page
section: contributing
title: Issues
permalink: /issues/
---

## Reporting Requirements

When filing an issue on the Spree project you must provide the following pieces of information:

* A comprehensive list of steps to reproduce the issue (on a clean install)
* The exact version of Spree you are running on (or git revision if using a GH branch)
* What you're *expecting* to happen compared with what's *actually* happening.

<span class="warning">
Your issue will not be investigated unless you provide all of the required information
</span>

_Please remember to format code using triple backticks (\```) so that it is neatly formatted when the issue is posted._

## When to File an Issue

You should file an issue if you have found (or suspect) a bug in the "core" functionality of Spree. If you have found a bug in one of the extensions, please file an issue with the appropriate extension project in GitHub. If you're not sure if the behavior you're experiencing is intentional just ask on the mailing list and someone will encourage you to file a ticket if your issue sounds like a bug (as opposed to a feature.)

If you think you've discovered a bug you can file an issue on the [Github issues](https://github.com/spree/spree/issues/) page for the Spree project.

## Labels

During the lifecycle of an issue it may be assigned one or more labels. The following is a list of labels grouped by phase.

_Please do not assign labels or create new labels to your issue. We will assign the appropriate labels to ensure your ticket is handled in the appropriate manner._

### Triage

Issues that are actively being investigated fall into this category. Once in progress an issue is either rejected or closed.

**Unverified**

This is the default label that will be applied by Spreebot whenever an issue is created in Github.

**Verified**

We manually verified and reproduced the issue. We might ask and encourage you to provide a [pull request](/pull_requests) to fix the problem reported.

**Reopened**

The issue has been reopened. This label will be applied automatically by Spreebot whenever an issue is reopened in Github.

### Rejected

Issues can be rejected for a variety of reasons. If your issue has been rejected you are encouraged to reopen it once you have addressed the reasons for rejection.

**Steps**

You need to provide a detailed set of steps to reproduce the problem. It should be possible for another developer to reproduce the problem using a clean install (no extensions or customizations) if they follow your steps and use the Spree version specified.

**Version**

Please include the exact version of Spree you are using (or git ref if you are working against a branch). We will need this information in order to verify the bug.

**Expected Behavior**

In additon to describing the observed behavior you need to describe how this differes from what you expect the behavior to be. Providing this information helps save us time when trying to reproduce your problem.

**Feature Request**

To discus a new feature for Spree please use the [spree-user mailing list](http://groups.google.com/group/spree-user) to discuss it, or open a [pull request](/pull_requests) with code for the new feature you would like to see in Spree.

### Closed

Issues in this category are no longer active and unlikely to be reopened.

**Stalled**

Any issue that is open for 14 days without actionable information or activity will be marked as "stalled" and then closed. Stalled issues can be re-opened if the information requested is provided.

**Not a Bug**

A determination has been made that the observed behavior is not a bug and therefore barring new information, the issue will not be fixed.

**Works For Me**

We could not reproduce this issue on a clean install.

## How We Prioritize Issues

Spree is a very large project with lots of activity. We try our best to respond to all of the questions and issues our users have.  We use the following criteria to prioritize issues:

* Does this bug effect the latest stable release?
* Are there details on how to reproduce the problem?
* Is there a patch associated with the issue?
* Is there a test included in the patch?
* Has someone else verified the bug?

We give highest priority to issues where the answer is "yes" to all of these questions. Next highest priority is for issues that answer "yes" to most of these questions, particularly the first few criteria.
