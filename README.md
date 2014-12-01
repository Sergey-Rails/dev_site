# Spree dev site

[Jekyll](http://jekyllrb.com/docs/home/) based developer website for [Spree](http://github.com/spree/spree)

## Run it locally

Install all the dependencies:

```shell
bundle install
```

Then run the local server, we set the baseurl to be an empty string so it will
be available at [http://localhost:4000](http://localhost:4000) without the
project-name suffix

```shell
bundle exec jekyll serve --baseurl ''
```

# Contributing

The Spree Dev Site is an open source project and we encourage contributions. Please review the
[contributing guidelines](http://guides.spreecommerce.com/developer/contributing.html)
before contributing.

In the spirit of [free software](http://www.fsf.org/licensing/essays/free-sw.html), **everyone** is encouraged to help improve this project.

# License

Spree is released under the [New BSD License](https://github.com/spree/spree/blob/master/license.md).
