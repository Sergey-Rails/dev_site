---
layout: page
section: policy
title: Issue Triage
permalink: /issue_triage/
---

Spree is an extremely popular open source project and as such, we deal with a large volume of reported issues. We have developed a standard policy to triage issues which must be followed consistently by all of our community volunteers.

## Moderators

Moderators are community volunteers that help with triaging the large number of Github issues as well as helping with eliminating spam on the mailing list. Moderators do not have full commit access and they are one step below core members in terms of their powers and responsibilities. Moderator is often a step towards full core team membership. Core team members also help with issue triage and the same policies apply to these individuals as well.

## Mutual Respect

There is one hard and fast rule when it comes to the Spree community and that is to always be respectful. This is a place where talented people can work with and learn from other dedicated professionals interested in a shared technical challenge. Whether you are filing an issue or responding to someone else's issue you need to be respectful. Otherwise you will quietly be ignored. This goes for the people running our community as well. Be professional, show respect and don't feed the trolls.

## Spreebot

Moderators do not have full commit access to the Github project but we have devised an automated solution known as [Spreebot](https://github.com/spree/spreebot) which allows moderators to help manage issues without requiring full commit access to the project. Spreebot helps us by listening to Github activity in the Spree project and automatically processing certain types of events according to our triage policy.

## New Issues

New issues are treated as follows:

#### **Unverified**

New issues are automatically given an 'unverified' label by Spreebot.

![Unverified label](/assets/unverified.png)

#### **Verified**

Moderators will review all unverified issues and attempt to verify them following the steps to reproduce supplied by the person reporting the issue. If the moderator is able to reproduce the problem then they can verify the issue by adding the following comment:

```
triage:verified
```

![Verified label](/assets/verified.png)

Spreebot will also automatically remove the 'unverified' label when this happens.

## Rejected Issues

It may not be possible for us to verify an issue. If issues do not contain 100% of the [required information](/issues) then they will be rejected. If an issue is rejected it does not mean that it's not a bug or that we won't eventually consider it. Rejection means that we will not attempt to verify your issue until you provide the required information.

<span class="warning">Don't be discouraged if we reject your issue. We will gladly revist the issue once you supply the required information.</span>

Whenever an issue is rejected, Spreebot will automatically add a detailed comment to the issue providing futher explanation as to why the issue cannot be accepted in it's current state.

![Steps comment](/assets/steps_comment.png)

There are a few specific reasons why your issue will be rejected. The following rejection labels will automatically be added by Spreebot once the issue is rejected as such by a moderator:

#### **Steps**

The issue is missing the necessary steps to reproduce the problem.

```
reject:steps
```
Spreebot will automatically close the ticket and give it the 'steps' label.

![Steps label](/assets/steps.png)

#### **Version**

All issues need to specify the version of Spree affected by the issue.

```
reject:version
```

Spreebot will automatically close the ticket and give it the 'version' label.

![Version label](/assets/version.png)

#### **Expected Behavior**

All issues need to specify not only the observed behavior but also how it differs from the expected behavior.

```
reject:expected_behavior
```

Spreebot will automatically close the ticket and give it the 'expected behavior' label.

![Expected label](/assets/expected_behavior.png)

#### **Address Feedback**

```
reject:address_feedback
```

Spreebot will automatically close the ticket and give it the 'address feedback' label.

![Expected label](/assets/address_feedback.png)

#### **Discussion**

```
reject:discussion
```

Spreebot will automatically close the ticket and give it the 'discussion' label.

![Expected label](/assets/discussion.png)


#### **Need specs**

```
reject:need_specs
```

Spreebot will automatically close the ticket and give it the 'need_specs' label.

![Expected label](/assets/need_specs.png)


## Closed Issues

Issues have an intentionally short lifecycle in our project. We need to focus on issues that have been verified and have the potential to be acted upon immediately. We need to be very aggressive in closing issues or it becomes impossible to stay on top of what is important.

<span class="warning">Don't be discouraged if we close your issue. It can always be reopened.</span>

Closing an issue simply represents an initial ruling by the moderator triaging this issue. For instance, if the moderator cannot reproduce the problem the issue will be closed. Issues can be reopened at any time an if there is new information to consider we will take that into consideration.

![Closed](/assets/closed.png)

The final decision on an issue is a group decision made by the core team after a public discussion about the merits of addressing it. These initial decisions are often overruled once there is sufficient debate and a chance build a  consensus from the community.

When an issue is reopened, Spreebot will automatically supply the appropriate label. The 'reopened' label will also be removed automatically whenever an issue is subsequently rejected or closed.

![Reopened label](/assets/reopened.png)

The following labels apply to closed issues:

#### **Works for Me**

The moderator was unable to reproduce the problem following the steps provided and using the specified Spree version.

```
close:works_for_me
```

Spreebot will automatically close the ticket and give it the 'works_for_me' label.

![Works for me label](/assets/works_for_me.png)

#### **Stalled**

The moderator has closed the issue because there has been no progress made on the issue in the last fourteen days. Issues will be kept open beyond fourteen days if there is an ongoing discussion or if there is a clear indication that someone is working on a possible solution.

Issues may also become stalled if ther are no moderators available or interested in helping to verify the issue. This situation should be rare, however, and we try to close issues proactively so that there is always someone able to focus on verifying a potential new issue.

```
close:stalled
```

Spreebot will automatically close the ticket and give it the 'stalled' label.

![Stalled label](/assets/stalled.png)

#### **Not a Bug**


```
close:not_a_bug
```

Spreebot will automatically close the ticket and give it the 'not_a_bug' label.

![Not a bug label](/assets/not_a_bug.png)
