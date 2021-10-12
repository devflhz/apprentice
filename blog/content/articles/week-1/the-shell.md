---
title: 💻 The Shell
tags: [course, shell, linux, week-1]
layout: post
url: articles/the-shell
author: Eduardo Flores
publishdate: 2021-10-10T14:23:00.000Z
summary: Tips and tricks about the shell.
---

Over the last few years I've been experimenting a lot with shell and shell scripting, this is something I really enjoy and have researched a lot about it.

When I was assigned to take this course the first thing I noticed was that the lecture was given by **Jon Gjengset**. He's been great teacher and I really enjoy learning from him and his [YouTube channel](https://www.youtube.com/channel/UC_iD0xppBwwsrM9DegC5cQQ), he's one of the persons I admire the most, he's a great teacher and a great developer.

As you might imagine by now, my interest for this course was immediately captured by the fact that **Jon** was teaching it and I was sure I would be able to learn something new.

I was right...

# The `cut` command.

35 minutes into the video I noticed a command I had never used before, the `cut` command.

This command is used to cut out sections from text and writing the result to the standard output. It works similarly to the `split()` function in programming languages, it's used to split a string into multiple strings and it can be saved as an array. You use a flag called `-d` or `--delimeter` to specify the delimiter and we access it by a flag called `-f` or `--field`.

# The root user.

- The root user has user id `0`.
- The `#` symbol is used to indicate to run the command as root or that the current shell is running as root.

# Kernel parameters.

Kernel paramters live inside the `/sys` directory and are represented as files, which means they can be used with almost every command.
This allows us to access kernel parameters from the command line and use them to configure our system.

# The `tee` command.

The `tee` command takes its input and writes it to a file, but also writes it to the standard output.

# The `xdg-open` command.

This command will open a file in the appropriate program for the file type.

If you open a `html` file with this command, it will open it in a web browser.
