---
layout: post
title:  "Opening Visual Studio Code from Command Line (Mac OS X)"
date:   2015-12-09 22:30:00
categories: visual studio code
author: Carlos R. Mendoza
<!-- permalink: -->
---

Recently I started trying out [Visual Studio Code](https://code.visualstudio.com/), and I must say I am impressed! It's open source, fast, and has built in debugging. It is in beta now, but I think it has a lot of potential to combine the speed of a text editor like [Sublime Text](http://www.sublimetext.com/) with some of the powerful tools found in full-fledged IDEs like [WebStorm](https://www.jetbrains.com/webstorm/).

Anyways, let's get to the point.

To configure your machine to open projects in Visual Studio Code from the terminal using the `code .`, follow the steps below.

1. Open your terminal, and enter `open ~/.bash_profile`. If the file doesn't exist, create it -- `touch ~/.bash_profile` -- and procceed to open it. *<font color="red">Note</font>*: if you are using **zsh**, then skip to step 2 and add the line of code found there to `~/.zshrc` instead.
2. In .bash_profile, add the following: `code () { VSCODE_CWD="$PWD" open -n -b "com.microsoft.VSCode" --args $* ;}` and save.
3. Restar your terminal.
4. Navigate to the project you wish to open and enter `code .`.
<br />
<br />
<div style="text-align: center;" ><iframe width="640" height="480" src="https://www.youtube.com/embed/UF7X6KJ6vBA?rel=0&amp;showinfo=0" frameborder="0" allowfullscreen></iframe></div>
<br />
<br />