---
layout: page
title: Rules and Guidelines
permalink: /rules/
---

This document will describe the rules and guidelines we use to either accept or
deny a pull request. Some rules warrant more discussion from the core team before
it get's accepted.


## Rules

### 1. Don’t decorate the state machine.
We are moving away from the complex and low performance state machine logic. We do not accept any new changes or usages for the statemachine logic.

### 2. No callbacks.
Similar to number 1 above, we are moving away from the heavily used callbacks to prevent the cascading touching and other low performance resulting in using these callbacks.

### 3. Public API changes will need justification.
The stable releases are named stable for a reason, let's keep it that way. Any public API (breaking) change needs proper discussion before accepting it. We will never merge these changes in the stable branches.

### 4. Limit (avoid) adding actions to controllers & models.
Use concerns or behaviour classes to add logic, we need thin controllers and small models.

### 5. Performance can’t take a hit.
No need to explain this :)

### 6. No additional queries.
See number 5.

### 7. Breaking other specs.
No pull request with breaking specs is getting in, make sure you don't break other specs as well.

### 8. Use of non-localized strings.
We need to make sure that every string in the system can be localized. So use the translation files.

### 9. Destruction or change data.
Be very very carefull here, every change that adds destructive methods or changes existing data needs to have a solid review before getting in.

### 10. Adding new gem dependencies.
We need te keep spree as light on dependencies as possible.

### 11. API endpoints need to proper authentication/authorization
Securtiy is major thing in ecommerce, make sure you use the supplied cancan authorization calls. TODO link to documentation here.

### 12. No more class_eval!
Since we dropped the ruby 1.9 support on the latest Spree master, there is no more excuse not to use the Model#prepend approach. [Sample on extending classes](http://guides.spreecommerce.com/developer/logic.html#extending-classes)
