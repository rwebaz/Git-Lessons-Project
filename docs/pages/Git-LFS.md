---
title: Git LFS
layout: default
excerpt: Update your development machine ports before installing Git LFS ...
hint: Place the intro paragraph ie.) the 'hypothesis' here ...
repo: Git-Lessons-Project
ver_date: 11-26-19
navigation_weight: 8
categories: page
---
{% include toc.md %}

## Macports dot org

> **Hint**. {{ page.hint }}

Go to the online Macports dot org guide.

- Navigate to Chapter 3. Using MacPorts C=> https://guide.macports.org/

- From the Terminal prompt of your user root directory

```liquid
{% raw %}
sudo port selfupdate
{% endraw %}
```

The Terminal will prompt for a password to set up a secure session.

Updating MacPorts base sources using rsync ...

Upon completion, update all of your ports ...

```liquid
{% raw %}
port upgrade outdated
{% endraw %}
```

Updating the ports tree

**Note**. The selfupdate action should be used regularly to update the local ports tree with the global MacPorts ports repository so you will have the latest versions of software packages available. It also checks for new releases of MacPorts itself, and upgrades it when necessary.

Next, from the global Terminal prompt, install **Git LFS**

```liquid
{% raw %}
port install git-lfs
{% endraw %}
```

Switch to the Terminal prompt for your repo ...

from the repo Terminal prompt


```liquid
{% raw %}
git lfs track '*.svg'
{% endraw %}
```

Responds ...

Tracking "*.svg"

Now when you go to your repository settings in the **Git Hub For Mac** program, you will see a reference `*.svg` has been placed in the **Git LFS** section.

As a result, all of the ( .svg ) files from this repo will possess a pointer to the remote **Git LFS server farm** where your ( .svg ) files for this repo will be housed and subsequently called.

And, when you review the repo from the Finder you will see a "cloud" icon now sits to the right of your ( .svg ) file name confirming a "cloud" service, in this case the **Git LFS** server farm has the original file under management remotely.

SVG files can get quite large.

For example, an large icon file converted to ( .svg ) can weigh in at well over a megabyte **MB**.

## Last Subtitle

More to come ...

***

**Note**. The above synopsis was derived from an article written by Alan Smith [[1](#ALANSMITH){:.red}].

1. {:#ALANSMITH}[Git LFS Training at GitHub Universe 2015 w Alan Smith](https://www.youtube.com/watch?v=l5SIbsy21jE){:title="Click to Review LFS Training at GitHub Universe 2015"}{:target="_blank"). Published by © 2015 [Githubuniverse.com](http://githubuniverse.com){:title="Click to Review GitHub Universe"}{:target="_blank"}.

***

{% include patreon-link.md %}
