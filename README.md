# Code Glossary for Udemy Unity course

This is a collection of some definitions for students of
https://www.udemy.com/unitycourse who have never written code
before and want a quick reference for what some of the common
programming terms mean.

This will always be a work in progress, so please let me know
if something is hard to follow, a term is missing, or anything
else you think could be improved.

It is hard for experienced programmers to notice when they are
using programming jargon, so I count on new coders to point out
the gaps.


## Introduction

*I didn't write this yet. I want it to include:*

 - how and why code is organized in files, classes, methods
 - very brief overview of compiling and compiler errors (the
   compiler is your friend, it wants to help you write correct
   code)


## `class`

*TODO: write this bit*

## member

A *member* is a piece of information or functionality that belongs
to a *class*. It is defined within the `class` code block.

In the following code, `myValue` and `DoSomething` are *members* of
`MyClass`.

```csharp
class MyClass {

  static int ourValue;

  int myValue;
  
  void DoSomething () {
    // code here to do something
  }
}
```

Some members belong to the *class* itself. These are called *static members*.
In the above example, `ourValue` is a static member (because it has the `static`
keyword in front of it).

Some members belong to an *instance* of the class. These are called *instance members*.
In the example above, `myValue` and `DoSomething` are instance members (because they
do not have the `static` keyword in front of them).


You can access a member using the `.` operator ("dot operator"). You write the name
of the *class* (for static members) or *instance* (for instance members) then a dot,
then the name of the member.

e.g. to get the static member `ourValue` from the class `MyClass`, write 
`MyClass.ourValue`. Here are some examples writing that to set the value
in `ourValue`, and to assign the value to a new variable named `something`

```
MyClass.ourValue = 5;
int something = MyClass.ourValue;
```



*TODO: add more information here (instance member usage examples, etc.)*

## `static`

*You may want to read what a class is, and what a member of
a class is, to help understand this concept.*

Use `static` on any *member* of a *class* to declare it as a
member of the whole class (a "static member") instead of a
member of an *instance* of a class (an "instance member").

Example usages:

```csharp
public static int NumberOfElephants;

public static void MakeAPancake () {
  Debug.Log("Yay! Pancakes");
}
```
