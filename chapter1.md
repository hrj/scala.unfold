---
layout: chapter
title: Introduction
next: chapter2.md
---

# Introduction

Before diving into Scala, let's step back a bit and survey the programming language landscape.

Please note that this is not intended to be a "war of the languages", and the analysis offered here is
possibly subjective. The intention is purely to provide a background to the newbie programmer,
before setting off deep into Scala land.

## The Language Landscape

There are hundreds of programming languages in use today and new ones are being designed all the time. No language is
perfect, that is, no language is suitable for every programming task. Each language
has its own set of tradeoffs and is suitable for a specific subset of applications. Let's look at some
popular languages to understand how Scala fits into this language ecosystem.

But before that, some definitions. You can skim through these if you are already familiar with half a dozen languages.

### Expression Types

One of the key factors in evaluating any programming language is the notion of expression types and how the
language deals with them. Examples of simple types are "integer", "float", "string", "boolean", etc. Examples
of more complex types are "class Person", or "class Shape", or "function that takes two integers and returns one string".

#### Strongly typed v/s Weakly typed
In `strongly typed` languages, each expression or stored value (cell) has a definite type, and it is an error
to access them with a different or incompatible type.

In `weakly typed` languages, some expressions or cells can be accessed as different types, based on the surrounding context.

Apart from this distinction of `strong` v/s `weak` typed languages, there is another axis to compare languages:

#### Statically typed v/s Dynamically typed
In `dynamically typed` languages, the type of a cell can change over the course of the program. Since the type
of a cell can change you don't have to specify the types (saving some keystrokes) and it affords more flexibility
to the designer of the application. It is easy to write small programs (scripts) in these languages, because you
don't have to pay the "type tax".

In `statically typed` languages, the type of a cell does not change over the course of the program. The compiler
for such a language is better able to reason about the program and its types; it is able to catch type
related errors at compile time and can also do a better job at optimisation.

Statically typed languages generally outperform the dynamically typed languages by [a factor of 4 to 50](http://benchmarksgame.alioth.debian.org/u32/which-programs-are-fastest.php),
and it is generally easier to write large programs in these languages, because the compiler can automatically perform the hard
work of type verification.

Further, some statically typed languages can infer the types automatically, thus reducing the burden of
specifying type annotations for every expressions / cell.

In the context of the above, let's examine some popular languages now.

### Level of abstraction
In low-level languages, the programmer is given full control of the processing environment (within the confines
of the Operating System ofcourse). This power and flexibility however requires more programmer discipline. Such languages
are suitable for writing performance-critical applications or system programs (such as device drivers).

In high-level languages, the processing environment is often abstracted out, so that the programmer need not
be bothered about these details and also so that code could be made portable across environments. These languages
often sport some convenient features to make programming quicker, faster, or more robust. They are suitable for
programming general purpose applications.

### Memory Management
In low level languages, the programmer needs to managed memory allocation and deallocation by themselves. This is
a particularly tricky task, and errors can lead to irrecoverable exceptions, or worse, security breaches.

In most high level languages, memory is automatically managed by the run-time environment thus reducing a huge
burden of the programmer.

### Object oriented programming (OOP)
`TODO`
Based on how real world objects behave.
Encapsulation
Inheritance


### C

The `C` Language is a low level language that gives a lot of flexibility and control to the programmer, and 
is thus suitable for writing system programs or writing performance critical sections. `C` lacks high level abstractions and
thus it is difficult to write and maintain very large applications in it.

For most purposes `C` is a statically and strongly typed language. However, it allows pointer conversions, pointer arithmetic
and low level access to memory, and when these are used, it becomes a weakly typed language!

### Java

The `Java` language is a high level language that has support for Object oriented programming. It compiles to a virtual machine
called the JVM (Java Virtual Machine).  The code executed by the JVM is called Java Byte Code. Because of the virtual machine layer
and its particular design, there are two benefits:
1. The code is portable across Processor Architectures and Operating Systems
2. Memory is managed by the VM automatically. The programmer doesn't have to allocate and free memory manually.
3. The combination of static typing and JIT compilation gives very good performance (for warm paths).

Both, Java and Java byte code are statically typed and strongly typed systems.

### Ruby & Python
These are dynamiclly typed high level languages. They have partial support for object oriented concepts (modules in Python and objects in Ruby).
However the OO support is not complete as there is no support for class inheritance.

### Lisp
`TODO`

### Haskell
`TODO`

### Scala
`TODO`

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
