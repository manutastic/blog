---
layout: post
title:  "Automatically test your database backups."
date:   2017-05-9 23:45:33 -0400
categories: jekyll
---
One of the issues of yesterday’s GitLab.com “database incident” is that most of their database backups weren’t being tested, and when they needed a restore, they discovered that most of the backup methods hadn’t been working.

Untested backup methods that turn out to be missing or broken are extremely common. I can’t fault them much because it’s a very easy mistake to make: most backups, by nature, never need to be restored from, so you never realize if something changes and they stop working… until it’s too late.

The solution is to frequently and automatically test backups by: