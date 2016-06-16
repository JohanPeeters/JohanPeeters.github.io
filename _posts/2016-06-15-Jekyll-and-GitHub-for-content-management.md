---
layout: post
title: Jekyll and GitHub for content management
---

I have written content management systems. I have used content management systems. Earlier attempts fetched content from a database and poured it into templates. Lately, I have been eschewing databases for building web sites with infrequent updates.

When your CMS receives a GET request, making a connection to a database to retrieve content is crazy expensive and then assembling the target page is crazy expensive. This is usually solved by caching the assembled page to serve subsequent requests.
