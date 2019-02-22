---
layout: post
title:  Vim And Rust
date:   2019-02-22 13:36:00 +530
categories: rust, vim
---

While programming in rust, I was beginning to type up a rather long subroutine. I wanted to make sure everything was compling file after every few lines. That's when I encountered the old frustration, having build using cargo on the command line, scrolling through errors and warnings, locating the file, get the line number for error or wargning, then go to vim and try to fix it, then go back to the console and find next error/ warning.

That all should be doable from vim. Some google searches went to nowhere. But, then I found the vim manual page for quickfix command while reading an answer on SO and voila! that was all I needed.

Here's the command to add "cargo build" as the make program in vim.
:set makeprg=cargo\ build

and then,
:mak

then,
:cope[n] to bring up the quickfix list

and, if you'd like the quickfix list to occupy full window size,
Ctrl+Wo

Now, navigating this quicklist the way you like is another beast.


