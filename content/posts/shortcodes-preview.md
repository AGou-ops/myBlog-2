---
title: "Shortcodes Preview"
date: 2019-03-04T16:01:23+08:00
lastmod: 2019-03-05T16:01:23+08:00
draft: false
tags: ["preview", "shortcodes"]
categories: ["docs", "shortcodes", "index"]
author: "AGou"
menu:
  main:
    parent: "docs"
    weight: 2
---


## What a Shortcode is

Hugo loves Markdown because of its simple content format, but there are times when Markdown falls short. Often, content authors are forced to add raw HTML (e.g., video `<iframes>`) to Markdown content. We think this contradicts the beautiful simplicity of Markdown's syntax.

Hugo created **shortcodes** to circumvent these limitations.

A shortcode is a simple snippet inside a content file that Hugo will render using a predefined template. Note that shortcodes will not work in template files. If you need the type of drop-in functionality that shortcodes provide but in a template, you most likely want a [partial template][partials] instead.

In addition to cleaner Markdown, shortcodes can be updated any time to reflect new classes, techniques, or standards. At the point of site generation, Hugo shortcodes will easily merge in your changes. You avoid a possibly complicated search and replace operation.

More details: https://gohugo.io/content-management/shortcodes/

<!--more-->

## blockquotes

Normal quote:
  This is a simple quote.

Quote with author:
  This is a quote with only an Author named Author2.

Quote with author and source:
  This is a quote from Author3 and source "source."

Quote with author and link:
  This is a quote from Author4 and links to https://www.google.com.

Quote with author, link and title:
  This is a quote from Author5 and links to https://www.google.com with title "Google."

Quote with author and a link longer than 32 characters, string is first cut at 32 characters then everything after the last forward slash is removed
  This is a quote from Author5 and links to https://twitter.com/CryptoGangsta/status/716427930126196737 which is longer than 32 characters.
  <br>And this is a new line in the quote with the HTML br tag.

Test from the Octopress blockquote page at: http://octopress.org/docs/plugins/blockquote/
  Over the past 24 hours I've been reflecting on my life & I've realized only one thing. I need a medieval battle axe.


## music

{{% music "http://39.99.144.153/remote.php/webdav/Don%20Diablo%20-%20On%20My%20Mind%20(Radio%20Edit).mp3" %}}

## gist(+1)

We can embed the gist in our content via username and gist ID pulled from the URL:

```
{{</* gist AGou-ops 5e0b2df2f0d23c65742a633ed0225cf6 */>}}
```

Display:

{{< gist AGou-ops 5e0b2df2f0d23c65742a633ed0225cf6 >}}

## expand
The Expand shortcode displays an expandable/collapsible section of text on your page. Here is an example

Yes !.

### Usage
this shortcode takes exactly one optional parameter to define the text that appears next to the expand/collapse icon. (default is “Click to expand”)

```
Yes !.
```

## youtube

{{< youtube w7Ft2ymGmfc >}}


## vimeo

{{< vimeo 146022717 >}}

## youku

