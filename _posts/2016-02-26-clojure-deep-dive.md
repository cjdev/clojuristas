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



### Forms and 
Expression evaluation
  Data structures evaluate to themselves
  Lists are special in that they evaluate/reduce to a value
    Function then Args
    Function appled to Args
    Eval / Apply
  Other kinds of Lists Generally called Forms or even Special Forms 
    are "these kinds of lists"
    What is a Form -> definition
    How do we use lists as a data structure ? - surpress execution

Expressions
  function followed by arguments -
  do it right (+ 1 2 3)
  do it wrong (1 2 3) 
  the List is our AST -> there compilation but nothing like Java or Scala here
  watch me create a list '(+ 1 2 3)
  watch me alter a list  (eval (cons / (drop 1 '(+ 1 2 3))))
  eval one then the other 

Forms/Special Forms

def
fn
defn
let
if
where

data 'types'
list
vector - unlike list in that access in constant time and wont be mistaken for "code"
hash-map
set


Basic functions

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

Try [clojure-docs online](http://clojure-doc.com)

