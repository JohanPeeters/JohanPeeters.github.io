---
layout: post
title: Jekyll and GitHub for web content management
---

I have written web content management systems and I have used content management systems. Earlier attempts fetched content from a database and poured it into templates. Lately, I have been eschewing databases for building web sites with infrequent updates.

When your CMS receives a GET request, making a connection to a database to retrieve content is crazy expensive and so is assembling the target page. Hence a database-backed CMS often caches the resulting page for the next request. 

Caching is a wonderful technique that has been used to great effect to improve performance of all sorts of systems. In fact, the web today has caches everywhere, in the browser, in the network and in the data center. But caching brings its own problems. Let's briefly review a couple: staleness and contention.

A cache entry is stale when it is not consistent with the authoritative source. In the context of a CMS, this means that content is updated but the system continues to serve the old content. There are basically 2 ways to avoid this: frequently expiring cache entries and invalidating them on update. The former solution is simple to implement but you need to set an expiry 
