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


## `class`

*TODO: write this bit*

## member

A *member* is a piece of information or functionality that belongs
to a *class*. It is defined within the `class` code block.

In the following code, `myValue` and `DoSomething` are *members* of
`MyClass`.

```csharp
class MyClass {

  int myValue;
  
  void DoSomething () {
    // code here to do something
  }
}
```

Some members belong to the *class* itself. These are called *static members*.
Some members belong to an *instance* of the class. These are called *instance members*.


*TODO: add more information here*

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
