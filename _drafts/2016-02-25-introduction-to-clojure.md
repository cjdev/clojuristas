---
layout: post
title: Introduction to Clojure
---

## Overview :

The clojuristas are a group of CJ devs who want to learn and play in Clojure.

Create an environment of free inquiry to learn and experiment. 

### What We Are:
- Clojure fans seeking other fans
- Enthusiats
- Geeks
- Good People having a Good Time with a LISP
- .... For the Brave and True

### What We are Not 
- Experts 
- \*Show offs 
- Propellerheads ... well maybe a little ;)

\* In German a "show off" is known as an *Alleskenner* ... betcha you didn't know *that* huh? ;)

### Proposed Format
Weekly talks are inspired by a chapters in the book [Clojure for the Brave and True](http://www.braveclojure.com/). Time to time we may opt to view many of the excellent videos on [YouTube](https://www.youtube.com/user/ClojureTV).

Practical experience being a fantastic Teacher, our hope is to do a lot of *in class* experimentation. Our aim is to : "talk at least as much as we code".

Learning by experimentation and getting fast feedback is essential in retaining and understanding the material. 

We invite you to type along as we experiment and even *run-the-show* time to time:

> We'd like to offer an experiment for a truly hands-on experience : volunteers may be asked to be our "fingers" while the presenter is the "mouth" guiding the discussion. Don't worry - we wont laugh at your typing as long you promise to not laugh at what comes out of our mouths! :)


Attendees are encouraged to type along and try the experiments in class as we go.

### Homework - bringing it all home...

Homework is meant to help re-enforce a set of topics: 
Each week you can if you choose show us your solutions and ask questions. Participants may chime in and offer alternatives.
This way we'll learn from each other.

GOAL : have code build and tested in travis-ci or cloudbees. 

### Tying it up
We'll try to follow the themes set in CFTBAT chapter by chapter but may leave some of the details to the reader if we don't have the time to cover it.

We hope you will feel comfortable to ask quesitons - while we wont have all the answers but we may know how and where to find it.

We hope you will find these sessions valuable - your feedback to help us help you (and ourselves) is greatly encouraged (stylistic, material)
If you have an idea please feel free not only to share but present it at the next meeting.


### Getting setup

Follow the the link to [Leinigen](http://leiningen.org) (its like maven) 

The installation instructions should be fairly clear - if not try something like this in your shell.

{% highlight shell %}

$> sh <(curl -S https://raw.githubusercontent.com/technomancy/leiningen/stable/bin/lein)

{% endhighlight %}

Or maybe

{% highlight shell %}

$> source <(curl -S https://raw.githubusercontent.com/technomancy/leiningen/stable/bin/lein) 

{% endhighlight %}

To fire up a REPL just type:

{% highlight shell %}

$> lein repl

{% endhighlight %}

And to exit and return to your shell

{% highlight shell %}

user=> exit

{% endhighlight %}




