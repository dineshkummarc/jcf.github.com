---
layout: post
title: "Hello Octopress"
date: 2011-10-07 20:11
comments: true
sharing: true
footer: true
sidebar: false
---

In case you haven't heard of [Octopress][], it's a fantastic static-site generator built on top of [Jekyll][].

I've been using Jekyll to build [jamesconroyfinn.com][] for sometime now and have been tickering with styles, layouts and features all along. Now with Octopress I feel like I've reached a point where I'm satisfied with the list of features, and the look of the site as a whole.

<!--more-->

## Features

Octopress offers some great features including:

* [HTML5 Video Tag][] - easily post images with class names and titles
* [Backtick Code Block][] - for simple lightweight code sharing
* [Code Block][] - for sharing code with titles and links
* [Include Code][] - embed code from your filesystem with a download link
* [Gist Tag][] - automatically downloads and embeds Github gists
* [jsFiddle][] - embeds code from jsFiddle
* [Image Tag][] - easily post images with class names and titles
* [Render Partial][] - insert any file into another post or page
* [Block Quote][] - generate beautiful, semantic block quotes
* [Pull Quote][] - generate CSS only pull quotes — no duplicate data, no javascript
* [Category Generator][] - generates archive pages for each blog category
* [Include Array][] - includes an array of partials specified in the _config.yml

## Configuration

Configuring your site when it's powered by Octopress is really simple.  After you clone your Octopress repo you're provided with a Rakefile full of helpful tasks to create new posts, new pages, download the provided theme, start customising, and then [deploy to an enviable list of hosts][].

I've tweaked things a fair bit but about 90% of the markup produced comes straight from Octopress.

## Tweaks

You can check out the changes I've made on [Github][] if you're interested.

You'll find I have overidden a number of styles to get the header looking the way I want, added links to the footer, attempted to hide the sidebar at all times, and injected a smattering of Helvetica Neue.

## Thanks

I have to thank [Brandon Mathis][] for all of his hardwork starting Octopress and to all those who have [contributed][] to making it what it is.

[Octopress]: http://octopress.org
[Jekyll]: https://github.com/mojombo/jekyll
[jamesconroyfinn.com]: http://jamesconroyfinn.com
[HTML5 Video Tag]: http://octopress.org/docs/plugins/video-tag/
[Backtick Code Block]: http://octopress.org/docs/plugins/backtick-codeblock/
[Code Block]: http://octopress.org/docs/plugins/codeblock/
[Include Code]: http://octopress.org/docs/plugins/include-code/
[Gist Tag]: http://octopress.org/docs/plugins/gist-tag/
[jsFiddle]: http://octopress.org/docs/plugins/jsfiddle-tag/
[Image Tag]: http://octopress.org/docs/plugins/image-tag/
[Render Partial]: http://octopress.org/docs/plugins/render-partial/
[Block Quote]: http://octopress.org/docs/plugins/blockquote/
[Pull Quote]: http://octopress.org/docs/plugins/pullquote/
[Category Generator]: http://octopress.org/docs/plugins/category-generator/
[Include Array]: http://octopress.org/docs/plugins/include-array/
[deploy to an enviable list of hosts]: http://octopress.org/docs/deploying/
[Github]: https://github.com/jcf/jcf.github.com
[Brandon Mathis]: http://brandonmathis.com/
[contributed]: https://github.com/imathis/octopress/network/members
