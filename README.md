# Worksheet 1: Getting Started with TypeScript

**Due: Monday, January 24, 11:59pm CDT**

For the conceptual worksheets in this course, we will provide a Markdown template in a repository that will be created for you through GitHub classroom.  You can clone this repository, directly edit your local copy with your answers, and then commit and push the file to complete the submission.  Alternatively, you can use GitHub's built-in Markdown editor and edit directly on your repository website without having to clone it locally.  If you are unfamiliar with Markdown syntax, then you can check out this [lovely guide provided by GitHub](https://guides.github.com/features/mastering-markdown/) before you get started.

*Do not make a copy of the provided Markdown template and submit that instead.* Our grading scripts will be looking for `README.md` within the root folder of your repository.  You should modify this template directly without changing the filename.



## Background

If you are new to TypeScript, you should familiarize yourself by reading the following chapters from the official handbook:

- [The Basics](https://www.typescriptlang.org/docs/handbook/2/basic-types.html)
- [Everyday Types](https://www.typescriptlang.org/docs/handbook/2/everyday-types.html)
- [Narrowing](https://www.typescriptlang.org/docs/handbook/2/narrowing.html)

Some of this information might appear pretty basic, but you will learn a lot about how TypeScript assigns static types to variables, objects, and functions and how it evaluates code execution paths to enforce strong typing.  You will also get a nice introduction to the syntax and pick up some handy tricks that are unique to this language, so don't skip them!

Here are a couple of questions to introduce you to some of the more unusual TypeScript syntax that will be useful in Assignment 1. Note that these are very brief questions in this first worksheet, so this may not take you long at all. That's ok, especially if you took the time to read the chapters above!



## Q1: Arrow Functions

In TypeScript, you can create anonymous functions that are not bound to an identifier.  They are typically used as inline functions that are used only once and do not require a name. Frequent uses for anonymous functions are callbacks and event handlers. 

In the following example, an anonymous function is defined that takes two numerical parameters.

```
var result = function(a:number, b:number) { 
    return a+b;
}
 
var c = result(22, 42);
```

TypeScript also provides a shorthand in the form of arrow functions.  The following code is equivalent to the above example:

```
var result = (a: number, b: number) => {
	return a+b;
}

var c = result(22, 42);
console.log(c);
```

One situation where you are likely to encounter arrow functions is when iterating through an array.  The array object has a `forEach` method that takes in an anonymous function as a parameter.  This function gets executed once for every item in the array, taking in the item as a parameter.  In the box below, write an arrow function that iterates through the array and outputs every element to the console:

```
var array = [1, 3, 5, 6, 8, 3];

// add your code here
```

You can quickly try it your code in a web browser using the [TypeScript Playground](https://www.typescriptlang.org/play/).  Note that you will you will need to open your web browser's developer console to see the output, which is typically activated using the F12 hotkey.



## Q2: Pizza

To be added.