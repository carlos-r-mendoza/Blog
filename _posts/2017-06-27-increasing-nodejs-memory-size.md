---
layout: post
title:  "Increasing Memory/Heap Size of Node.js"
date:   2017-06-27 11:20:00
categories: nodejs, node, javascript
author: Carlos R. Mendoza
<!-- permalink: -->
---

By default, Node sets a memory/heap size limit that is under 2 GB. This default can be changed by passing in a value in megabytes (MB) when starting a Node server using the following option:

`--max_old_space_size=<heapSizeInMB>`

Thus, the command below will start a server with a heap size of up to 4 GB.

`node --max_old_space_size=4000 scriptThatStartsServer.js`
