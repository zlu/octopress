---
layout: post
title: "Commandline Pretty JSON Print"
date: 2012-07-19 14:37
comments: true
categories:[tools, linux]
---

We often deal with viewing JSON documents in command line such as using curl against a server that returns JSON response.
It is hard to read.

[jsonpp](https://github.com/jmhodges/jsonpp/) comes to rescue.

On OS X, simply issue `brew install jsonpp`

{% codeblock lang:bash %}
zlu@zlu-mba:~/projects/perch/perch-api (master *)$ curl --user foo@bar.com:abc123 http://localhost:3000/users
[{"_id":"500859f1827bc70b84000001","created_at":"2012-07-19T12:03:22-07:00","email":"zlu@perch.co","facebook_access_token":null,"facebook_access_token_expiration":null,"facebook_id":null,"family_id":null,"first_name":"zhao","last_name":"lu","phone_number":null,"updated_at":"2012-07-19T12:03:22-07:00"},{"_id":"500864a1827bc710a9000004","created_at":"2012-07-19T12:48:49-07:00","email":"foo@bar.com","facebook_access_token":null,"facebook_access_token_expiration":null,"facebook_id":null,"family_id":null,"first_name":"foo","last_name":"bar","phone_number":null,"updated_at":"2012-07-19T12:48:49-07:00"}]
{% endcodeblock %}

After piping through jsonpp

{% codeblock lang:bash %}
{% endcodeblock %}
