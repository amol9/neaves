---
layout: post
title:  Jekyll Markdown Issue
date:   2019-02-22 13:40:59 +530
categories: jekyll
---

I was editing and testing a simple jekyll site, when, the post content on the index page started showing up raw (markdown not processed). I was playing around with config and index html, so, I tried a little "undo" to try to figure out the cause of error. But, nothing :(

The html for post content was like this:
> <p> {{ post.content }} </p>

It was getting a little frustrating, so I sat back a little and tried to think.

Thought of just clearing the "_site" dir and rebuilding everything. Thankfully, jekyll provides a command for it:

> jekyll clean
and then
> jekyll serve

And, miracle!! it worked. The post got rendered fine.


