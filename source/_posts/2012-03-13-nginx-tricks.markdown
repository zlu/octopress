---
layout: post
title: "Nginx Tricks"
date: 2012-03-13 09:19
comments: true
categories: [Nginx]
---

Test configuration change without restarting Nginx

nginx -t (sudo)

restarting working process

kill -HUP `cat /var/run/nginx.pid` (replace nginx.pid with your system)

log file full

cat /dev/null | sudo tee /var/log/nginx/error.log

then reopen log file

kill -USR1


