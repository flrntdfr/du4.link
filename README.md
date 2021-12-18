# Introduction

This is a plain HTML static URL shortener built with [Jekyll](https://jekyllrb.com).

# How to use it

**Preparation**

1. Get your own domain name: `domain.tld`.
1. Fork the repo.
1. Update `CNAME` with your domain name.
1. Update `_config.yaml` with your information.
1. Update `index.md` with your information.
1. Enable github pages for the repo.

**Shorten URLs**

1. Let's say you want to shorten: `https://sub.other-domain.com/2021/01/article.html`.
1. Let's say you want it to be `domain.tld/article`.
1. Create an HTML file under `_URLs` named as the permalink: Here `article.html`.
1. The content of this HTML page is:

```yaml
---
layout: redirect
# Time in seconds before the redirect.
time: '0'
# The target of the redirect.
target: "https://sub.other-domain/2021/01/article.html"
---
```

1. git add, commit, push.
1. Visit `domain.tld/article` and you'll be redirected.

# Features

- :white_check_mark: Plain HTML URL shortener
- :white_check_mark: Lightweight
- :white_check_mark: Faaaaast
- :white_check_mark: Free to host on github.com

- :negative_squared_cross_mark: No CSS, No JS
- :negative_squared_cross_mark: No database
- :negative_squared_cross_mark: No webserver
- :negative_squared_cross_mark: No loadbalancing
- :negative_squared_cross_mark: No analytics
- :negative_squared_cross_mark: Blockchain and AI free

