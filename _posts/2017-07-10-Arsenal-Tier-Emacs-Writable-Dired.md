---
layout: post
title: "Arsenal-tier Emacs: Mass Rename"
date: 2017-07-10 18:21:03 -0700
categories: emacs
---

Lets rename a folder of annoying Twitter `.png-orig` and `.jpg-orig`
files to what they should be--in less than five seconds!

![Renaming of an entire folder in no time at all](/assets/Mass-Rename.gif "Beep boop, renamed!")

<!-- more -->

# So, WTF did I just see?
You just saw an entire folder get renamed--using something called "Dired".

Emacs has a built-in-file manager, which doesn't sound very impressive
until you realize that you can edit folders like text files! All I did
above was simply find and replace "`-orig`" with nothing and
save. Simple as that!

![Find and replace](/assets/Dired-Rename.gif "It's all text!")

# How can I do this too?
In Emacs, `C-x C-f` [^1] lets you open files and folders... And when you
open a folder, you are placed in "Dired"; the mode you saw me use
above.

![Navigating to a folder](/assets/Dired1.png "Hit Tab a lot, nearly everything in Emacs does tabs a lot")

By default, Dired is read-only to stop you from making sweeping
changes to your folders (Imagine running across this without knowing
what you're doing!), but you can turn that off with `C-x C-q`. It
indicates you have done this in the bottom line.

![The bottom line shows you can edit!](/assets/Dired2.png "Uh oh")

After that, you can edit the folder as if it is a text file, using
whatever style of editing you prefer. When you are done, you can save
your changes to the folder by simply saving the buffer as if it were a
normal text file--or by hitting `C-c C-c` like the text at the bottom
suggests.

![Modifications!](/assets/Dired3.png "Macros work really nicely here too!")

...and that's it! Now you wield the power of mass-renaming!

[^1]: `C-x C-f` is Emacs-speak for `[Ctrl] + [X]`, then `[Ctrl] + [F]`.