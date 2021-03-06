---
title: How to use shorten GitHub URLs and create vanity URLs
post_date: on November 10, 2017 at 01:12 am
layout: post
description: Use git.io service to shorten GitHub URLs, and create vanity URLs
image: https://cdn.abraham.gq/blog/2017/november/git.jpg
web: https://blog.19cah.com/2017/11/10/how-to-shorten-urls-on-github.html
---

Suppose you want to shorten the URL to a particular location on GitHub, (the service for shorting URLs only works with Github URLs, so you cannot use it to external sites). Or perhaps you want to create a vanity URL that goes directly to your GitHub profile, e.g. [git.io/19cah](https://git.io/19cah). You can use [Git.io](https://git.io): GitHub URL Shortener.

 To shorten a URL, open your command prompt (via Git Shell) and type in

 ```
$ curl -i https://git.io -F "url=https://github.com/19cah" -F "code=19cah"
```
Where
```
-F "code=vanity"
```
For example `19cah`, that is my Github username, but you can use whatever you want.
Then you will recive in the response your shorten URL!
```
Location: https://git.io/v5hxi
```
To create a vanity URL to your profile or URL you need to add `#` at the end of your profile or the url,
```
$ curl -i https://git.io -F "url=https://github.com/19cah#" -F "code=19cah"
```
Now you'll recive in the respose
```
Location https://git.io/19cah
```
And that's all

### Check some of the shorteners that I own redirecting to my profile:

* [git.io/19cah](https://git.io/19cah)
* [git.io/abraham](https://git.io/abraham)
* [git.io/carlos](https://git.io/carlos)

You can use it to shorten your repositories, so it will be easy to share.

[![GitHub followers](https://img.shields.io/github/followers/19cah.svg?style=social&label=Follow)](https://github.com/19cah)
