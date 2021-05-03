---
layout: post
title: Add a Little Fun to the Shell
---

It takes as little as to write the command [_fortune_][1]{:target="_blank"} within the startup script [_.bashrc_][2]{:target="_blank"}, which is a hidden text file in the home folder.

All we get is to see some funny sayings every time we open up a Bash shell.

First, let's install fortune and try it.

```
$ sudo apt-get install fortune
```

```
$ fortune
You'll never see all the places, or read all the books, but fortunately,
they're not all recommended.
```

Second, put the command `fortune` to the last line of .bashrc using _nano_ or any other text editor.

```
$ nano $HOME/.bashrc
```

Want to make it funnier?

Let's install [_cowsay_][3]{:target="_blank"}, and make it work together with fortune.

```
$ sudo apt-get install cowsay
```

```
$ fortune | cowsay
 _________________________________
/ You will engage in a profitable \
\ business activity.              /
 ---------------------------------
        \   ^__^
         \  (oo)\_______
            (__)\       )\/\
                ||----w |
                ||     ||
```


[1]: https://en.wikipedia.org/wiki/Fortune_(Unix)
[2]: https://en.wikipedia.org/wiki/Bash_(Unix_shell)#Startup_scripts
[3]: https://en.wikipedia.org/wiki/Cowsay
