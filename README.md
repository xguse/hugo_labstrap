# labstrap 

labstrap is a double-column theme for [Hugo](http://gohugo.io/).
It is modified from [dim0627](https://github.com/dim0627)'s [Beg](https://github.com/dim0627/hugo_theme_beg) theme which, in turn, was inspired by [kAworu/octostrap3](https://github.com/kAworu/octostrap3).

I have added (will continue to add) features and structure that I find useful for keeping notes pertaining to my research.

It is a work in progress and __no one__ should probably ever use it -- including _me_.  But I have always been a bit stubborn.

![Beg Screenshot](https://github.com/xguse/hugo_labstrap/blob/develop/images/screenshot.png)

## Features

* Google Analytics
* Disqus
* SNS Links(Facebook, Twitter, GitHub)
* Share Button
* Tagging
* Related Post
* MathJax support

# Installation

    mkdir themes
    cd themes
    git clone https://github.com/xguse/hugo_labstrap.git labstrap
    
## Build with labstrap

    hugo server -t labstrap

# Configuration

## config.yaml ##

``` yaml
---
BaseUrl: "http://example.com"
LanguageCode: "en-us"
Title: "Rad Site That Uses LABSTRAP!"

Params:
  Author: "Gus Dunn"
  DateForm: "Mon, Jan 2, 2006"
  GoogleAnalyticsUserID: "your_deets"
  Facebook: "your_deets"
  Twitter: "your_deets"
  Github: "your_deets"
  ShowRelatedPost: True
  Disqus: "your_deets"
  SyntaxHighlightTheme: "solarized_light.min.css"

Indexes:
  tag: "tags"

permalinks:
  post: /blog/:year/:month/:day/:slug/

MetadataFormat: "yaml"
...
```

## example post ##


    ---
    date: "2015-05-15T14:34:06-04:00"
    draft: true
    title: "init"
    tags: ['x','y']
    categories: ['intro']
    ---

    # Hello... World? #

    \*cough cough\* is this thing on?

    # MathJax #

    Does this render: `$\mathbf{F} = \frac{\mathrm{d}\mathbf{p}}{\mathrm{d}t} = \frac{\mathrm{d}(m\mathbf v)}{\mathrm{d}t}$` ?

    # Code #


    ```python
    # lets use MUCH spam here
    spam = 'yes, please'
    eggs = True
    while eggs:
        print("Would you like spam with that?")
        print("Spam?! {answer}!".format(answer=spam))
    ```



# Contact me

Please mail to `gus.dunn@yale.edu`.
