---
layout: page
section: policy
title: Code Style
permalink: /code_style/
---

We follow the [Thoughtbot Styleguide](https://github.com/thoughtbot/guides/blob/master/style/README.md)
. This will be enforced for every pull request. We use [HoundCI](https://houndci.com) for that, so when
you violate a style rule there will be a comment on that specific line in your pull request.

Before you send a pull request, there are a few things that you can do yourself
to make sure that the rules are not broken.

## Rubocop
HoundCI uses [Rubocop](https://github.com/bbatsov/rubocop) to check for ruby syntax,
we added the [Rubocop rules](https://github.com/spree/spree/blob/master/.rubocop.yml)
in Spree so you can run the checks manually before submitting a pull request.
See the Rubocop [documentation](https://github.com/bbatsov/rubocop#basic-usage) on how to run it locally.
