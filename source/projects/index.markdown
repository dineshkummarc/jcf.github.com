---
layout: page
title: "Projects & Contributions"
date: 2012-03-24 19:20
comments: false
sharing: true
footer: true
---

I've contributed to a number of software projects, and strive to give
something back at every possible opportunity.

Here is a list of some of the things I've been able to do to help out.

## [WebMock]()

**Maintainer & [Contributor](https://github.com/bblimke/webmock/contributors)**

[WebMock]() is a very useful Ruby library that makes it easy to test the
way your application interacts with other web-based services.

I maintained the library while [Bartosz]() was unable to dedicate time
to the project, and contributed a few improvements here and there.

## [Git TextMate Bundle]()

**Maintainer**

I no longer maintain the [Git TextMate Bundle] but did so for around a
year.

As I haven't used TextMate in over two years, I can't dedicate the time
required to support and develop the bundle.

If anyone is interested in taking over development please do [get in touch](mailto:james@logi.cl?subject=Git TextMate Bundle).

## [Slim.growlStyle](https://github.com/jcf/Slim.growlStyle)

{% img left http://f.cl.ly/items/2j2a3e3K1k3C1p1k0n0O/slim-shot-v2.png %}

I built a custom style for [Growl](http://growl.info) some time ago, as
I had a small screen and a lot of notifications.

It's available to [download](https://github.com/jcf/Slim.growlStyle/downloads)
from Github if you'd like to use it or see how it's made.

## [jQuery Expandable](https://github.com/jcf/jquery.expandable)

This is a small jQuery plugin I built in a previous life to make it
trivial to hide and reveal large amounts of content. I decided to open
source it in case anyone else found it useful.

It's probably two years old and comes with **zero** test coverage, but
still works in most browsers.

There's a [demo](http://jamesconroyfinn.com/jquery.expandable/) where
you can see the code in action.

## Useful Snippets

### [Dotfiles]()

I've been sharing my [Dotfiles]() for a long-time now and there are some
useful snippets in there.

### [Propane Customisation]()

I use [Propane]() and Campfire quite a lot. If you're interested in
doing the same this is a good starting point.

{% img http://f.cl.ly/items/3Q1S3k0t1E0E07141A0N/propane-preview.png %}

## Backport ActiveRecord's Pluck method

A colleague of mine wanted to be able to use
[pluck](http://api.rubyonrails.org/classes/ActiveRecord/Calculations.html#method-i-pluck)
in a Rails 3.1 application, which couldn't be upgraded. I backported the
method for him in this [gist](https://gist.github.com/1781411).

We never used the code in production, because we refactored the use of
pluck out, but it's there if anyone wants it.

## Rotate Logs on OS X

OS X comes with [newsyslog]() which helps rotate your log files, or
simply truncate them if you wish as I do.

The configuration file I keep in `/etc/newsyslog.d/rails.conf` can be
found in this [gist](https://gist.github.com/1451317).

## Email Validation in Rails

I wrote a reusable email validator that I used in a few Rails
applications and threw it in to a [gist](https://gist.github.com/1188367).

It's in a gem too, although it's not stable enough to share at the
moment.

## Relative Timestamps

If you need to convert parsable timestamps in to relative times in a
client-side or Javascript-based application I implemented a solution
that can be found in this [gist](https://gist.github.com/1063575).

## Small Contributions

### [RVM](https://github.com/wayneeseguin/rvm/commits/master?author=jcf)

- Added the `current` command to output the current Ruby version and the
  gemset in use.
- Fixed ZSH completion.

### [Handlebars](https://github.com/wycats/handlebars.js/commits/master?author=jcf)

- Added support for double quotes back in the very, very early days.

### [Guard RSpec](https://github.com/guard/guard-rspec/commits/master?author=jcf)

- Added initial support for using DRB.
- Added a first-version of filtering the list of specs to run (for RSpec
  1 users).


[WebMock]: https://github.com/bblimke/webmock
[Bartosz]: https://github.com/bblimke
[Git TextMate Bundle]: https://github.com/jcf/git-tmbundle
[Dotfiles]: https://github.com/jcf/dotfiles
[Propane Customisation]: https://gist.github.com/1942526
[Propane]: http://propaneapp.com/
[newsyslog]: http://developer.apple.com/library/mac/#documentation/Darwin/Reference/Manpages/man8/newsyslog.8.html
