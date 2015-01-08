---
layout: page
section: policy
title: Code Style
permalink: /code_style/
---

## Ruby Styleguide and code quality

We follow the [Thoughtbot Styleguide](https://github.com/thoughtbot/guides/blob/master/style/README.md). This will be enforced for every pull request. We use [HoundCI](https://houndci.com) for that, so when you violate a style rule there will be a comment on that specific line in your pull request.

Before you send a pull request, there are a few things that you can do yourself to make sure that the rules are not broken.

### Rubocop
HoundCI uses [Rubocop](https://github.com/bbatsov/rubocop) to check for ruby syntax, we added the [Rubocop rules](https://github.com/spree/spree/blob/master/.rubocop.yml) in Spree so you can run the checks manually before submitting a pull request.
See the Rubocop [documentation](https://github.com/bbatsov/rubocop#basic-usage) on how to run it locally.

## CodeClimate code quality
We also run [CodeClimate](https://codeclimate.com/github/spree/spree) on all pull requests, low quality code needs to be refactored before we consider accepting the pull request.

## Ruby documentation with YARD
Add comments to the public interface in the ruby files with YARD, for usage see the [YARD Getting Started](http://www.rubydoc.info/gems/yard/file/docs/GettingStarted.md) page.

## Bullet
The [Bullet](https://github.com/flyerhzm/bullet) gem is available in the sandbox. That way you can test if your changes
introduce performance problems. To use it generate a sandbox and run it on your
localmachine. You will see the bullet reporting on screen, including suggestions
on how to improve the performance issue detected.
