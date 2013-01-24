---
layout: chapter
title: Getting started with Scala
prev: chapter1.md
next: chapter3.md
---

# Installation

## Installing a Java Runtime Environment
You need to install a Java Runtime Environment (JRE) before you can work with Scala.

Instructions for installing a JRE abound on the internet.

## Installing Scala
Download the Scala distribution for your platform from [here](http://www.scala-lang.org/downloads). The latest
version as of this writing is 2.10.0.

## Installing Eclipse (optional)
The [Eclipse](http://eclipse.org) IDE is a popular and free IDE for Java. Scala support is available
as a plugin. You need to install [the Scala plugin](http://scala-ide.org/) from within Eclipse.

Apart from working with Scala projects, the Eclipse-Scala plugin has one great feature called `Scala Worksheets`.
This offers a convenient way to learn Scala and is described in detail below.

# Running Scala programs

## REPL
The Read-Eval-Print-Loop (REPL) offers an interactive way to enter Scala expressions and to evaluate them instantly. The result
of evaluting an expression is printed below the expression and can be reused in other expressions.

To start the REPL, execute the `scala` program with no arguments. It will print something like:

```
Welcome to Scala version 2.9.2 (OpenJDK Server VM, Java 1.6.0_24).
Type in expressions to have them evaluated.
Type :help for more information.

scala> 
```

In the prompt shown above you can enter Scala expressions. For example, try entering `3 * 4`:

```
scala> 3 * 4
res0: Int = 12
```

The REPL will show the result of evalating `3 * 4` and also its type. This result will be automatically
assigned the symbol `res0` which can then be used in other expressions if desired. For example,
you could now evaluate `res0 * 2` and get the following output:

```
scala> res0 * 2
res1: Int = 24
```

## Scripts
If you pass a `.scala` file as an argument to the `scala` program, Scala will both compile and run
the `.scala` file. This is very useful for writing scripts (which are small programs)
than having a separate compilation and run phase.

Such `.scala` files which can be executed instantly have certain conventions. The entire body
of such a file is implicitly wrapped by Scala inside a `Main` object and executed automatically.
(We will learn about objects later; so don't worry about it if you don't understand what that means).

Try saving a file called `greet.scala` with the following contents:
``` scala
println("Hello world, I am a tiny script.")
```

When you invoke `scala greet.scala` you should see the greeting printed on `stdout`.

## Complete programs
TODO

## Worksheets
One great feature of the Eclipse-Scala plugin is `Scala Worksheets`. These are special files 
that get evaluated as soon as you save them. The evaluation results are shown right
beside the expression. This feature is very convenient while learning and exploring Scala.

