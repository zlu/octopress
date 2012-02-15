---
layout: post
title: "RubyMine and PivotalTracker Integration"
date: 2012-02-14 20:32
comments: true
categories: 
---

**Task Server** is a lesser known feature in RubyMine.  You can enable PivotalTracker (PT) integration by adding
PT project as a Task Server.

Press cmd + , to open Preferences.  Type task to see this panel:

{% img http://cl.ly/0q2Z231T2P3x452L0O1W %}

Add PivotalTracker project by supplying project ID and api token.

Now every story can be easily turned into a RubyMine changelist.
Press cmd + shift + a, and type task.  Select open task.  Type part of the story to see a list of matched tracker stories.

{% http://cl.ly/0p3L1L430g010Z11322T %}

Select the desired story to work on and check start story.  Now every change will be in this change list and RubyMine will
autostart the story.

Let's say you TDD'ed and finished the story.  Press cmd + k to open changelist view.

{% http://cl.ly/3S3S08072n271t0S231g %}

You will see that commit message has been filled with story text.  Commit the change and RubyMine will automatically
finish the story.  How cool is that?  Now try to do that in Emacs or VI, I dare you :P

P.S. I like Emacs.