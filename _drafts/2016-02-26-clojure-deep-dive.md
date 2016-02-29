---
layout: post
title: Clojure Deep Dive
---

### What's up? Clojure for the Brave and True - Chapter 03


### Digression 1 :  Everything is an Expression 

- Clojure differs from many languages in that it is based on expressions.
- Expressions are easier in principal to comprehend.
- All Expressions reduce to a value.
- Expressions in LISPs (like Clojure) are *expressed* in terms of `lists` or simple values.
- What we call *execution* in imperative languages is referred to as  *function application* or *reduction*.

{% highlight clojure %}
=> () ;; and there it is .... any questions? ;)
{% endhighlight %}

Simple expressions - things that evaluate to themselves

{% highlight clojure %}
user => ()
user => "Hello Rich Hickey"
user => [1 2 3]
user => '()
user => '(1 2 3)
user => :turtles
user => true
{% endhighlight %}

### Evaluation
Lists and Forms (coming next) are the context in which values are e-valuated. 

*Expressions* that are 'executed' are simply data in a list

Clojure syntax can be summed up as a: 

> List whose head is a function followed by args

Thats it. No Precedence. No AST. *You* build the AST.

The consequences of this are enourmous: the lines of code and data suddenly become blurred. It means `code` can be manipulated as `data` at compile or runtime. 

Lets try it out

{% highlight clojure %}

;; fire up the repl and type some values 
;; now lets create a vector
;; now a list ... what happend?
;;  suppress the list evaluation with a tick  '
{% endhighlight %}

### Forms and [Special Forms](http://clojure.org/reference/special_forms)

What is a Form?

A LISP  form is a LISP datum that is also a program, that is, it can be evaluated without an error.
 \-- robbed from StackOverflow which is good enough I guess...


- Every LISP has a basic set of *primitives* that defines the language.
These are called "Special Forms". Unlike regular forms a programmer does not define or manipulate the datum like regular forms. Instead they are defined and provided by the language itself.


- We'll introduce a subset of these 
-- quote
-- if
-- do 
-- let
-- def
-- fn
-- defn (def + fn)
-- there are others : var, loop, recur, try , throw - we will get to these later.

- Lets try each of the above

- For a list let's do it wrong then correctly 
-- You'll see a lot of these in the beginning

Expressions
  function followed by arguments -
  do it right (+ 1 2 3)
  do it wrong (1 2 3) 
  the List is our AST -> there compilation but nothing like Java or Scala here
  watch me create a list '(+ 1 2 3)
  watch me alter a list  (eval (cons / (drop 1 '(+ 1 2 3))))
  eval one then the other 

Basic Data Structures.

list
vector - unlike list in that access in constant time and wont be mistaken for "code"
hash-map
set


A few Basic functions 

inc / dec 
str
get
get-in
cons
assoc
assoc-in
conj

nil?
true?
false?



### Getting Help 
{% highlight clojure %}
; try running (doc *something* )  on these...
; find-doc
; source
; apropos
; type 
;
; for instance .....
user => (doc doc)
;
; now try using the source 'function'
;
;
{% endhighlight %}

Try [clojure-docs online](https://clojuredocs.org)

