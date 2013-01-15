---
layout: chapter
title: Introduction
next: chapter2.md
---

# Introduction

Scala is a multi-paradigm language that compiles to JVM (Java Virtual Machine) bytecode, and hence programs written in Scala
are portable across systems that run the JVM.

## The Language Landscape

There are hundreds of programming languages in use today and new ones are being designed all the time. Each language
has its own set of tradeoffs and is suitable for a specific subset of applications. We will survey some of
the popular languages to understand where Scala stands among these.

### Expression Types

One of the key factors in evaluating any programming language is the notion of expressions types and how the
language deals with them. Examples of simple types are "integer", "float", "string", "boolean", etc. Examples
of more complex types are "class Person", or "class Shape", or "function that takes two integers and returns one string".

In `strongly typed` languages, each expression or stored value (cell) has a definite type, and it is an error
to access them with a different or incompatible type.

In `weakly typed` languages, some expressions or cells can be accessed as different types, based on the surrounding context.

Apart from this distinction of `strong` v/s `weak` typed languages, there is another axis to compare languages:

In `dynamically typed` languages, the type of a cell can change over the course of the program. Since the type
of a cell can change you don't have to specify the types (saving some keystrokes) and it affords more flexibility
to the designer of the application. It is easy to write small programs (scripts) in these languages, because you
don't have to pay the "type tax".

In `statically typed` languages, the type of a cell does not change over the course of the program. The compiler
for such a language is better able to reason about the program and its types; it is able to catch type
related errors at compile time and can also do a better job at optimisation.

Statically typed languages generally outperform the dynamically typed languages by a factor of varying from
[4 to 50](http://benchmarksgame.alioth.debian.org/u32/which-programs-are-fastest.php), and it is generally
easier to write large programs in statically typed languages, because the compiler can automatically perform the hard
work of type verification.

Further, some statically typed languages can do type inference automatically, thus reducing the burden of
specifying a type annotation for every expressions / cell.

In the context of the above, let's examine some popular languages now.

### C

The `C` Language is a low level language that gives a lot of flexibility and control to the programmer, and 
is thus suitable for writing system programs or writing performance critical sections. `C` lacks high level abstractions and
thus it is difficult to write and maintain very large applications in it.

For most purposes `C` is a statically and strongly typed language. However, it allows pointer conversions, pointer arithmetic
and low level access to memory, and when these are used, it becomes a dynamically and weakly typed language!

### Java

### Python & Ruby

### Lisp

### Haskell

### Scala

## Why choose Scala?

### Features at a glance

* Statically typed and strongly typed => better tool support
* Higher ordered functions and closures
* Pattern matching constructs
* Seamless integration of Object oriented and Functional programming paradigms
* Covariant types and a comprehensive collection library with covariant types
* Type inference
* Compiles to JVM => portable to all systems that support JVM
* Binary compatible with Java and other JVM based languages
* Macros
* Concise and familiar syntax based on "curly braced" languages.
