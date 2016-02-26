---
layout: post
title: Clojure Deep Dive
---

### Welcome to Clojure for the Brave and True - Chapter 03

### What we'll cover more or less

The Humble List
> ()
Everything is an expression
  Define

Simple expressions

> "hello Rich"
> 1
> [1 2 3]
> ()

Getting Help 
doc
find-doc
source
apropos
clojure-docs online
type

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





