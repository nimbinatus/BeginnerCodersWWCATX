[Back to the index](/BeginnerCodersWWCATX)

# Objects and OOO with Python

_A Primer for Women Who Code ATX_

## Catching up on Python

Python is a programming language. In its most basic form, we use variables and functions just like in algebra. If you can think in variables in math, you can follow Python code. You may find yourself looking for references a lot of the time, but the basics really are just math.

We create and use _classes_ and _methods_ to work with Python code (though you certainly can stick to functions and variables, but we're talking object-oriented today!). In all of these cases, we work with _objects_.

## What do you mean by "object"?

An object in programming is essentially a thing that can have actions done to it. An object can be defined. An object can be used. An object can be assigned to another object (woah, don't go down that rabbit hole yet!).

When we say objects can be defined, we mean that we can assign an object to a variable and use the variable in our code. We can pass objects to other objects through function calls.

### Deep dive

There are templates called classes for every object; remember that you can create a class yourself. These template classes are baked into Python. There's a generic "class" object, for example, that is used to create every class. Look up the class for an object by calling `.__class__`.

## Everything is an object

Did you know everything in Python is an object? Yes, every single thing in Python is considered an object, from the string that you input to the class that groups variables and methods/functions together to the classes themselves. The main thing you need to know is that everything you see in Python code is an object. As you work more with Python code, this idea will start to sink in (slowly, trust me). As long as you remember that everything is an object, you will start to understand what it means when you keep using different bits of code over time.

## Object-Oriented Thinking

When we talk about thinking in an object-oriented way, we are talking about how we design programs. There's _procedure-based_ programming, which thinks in functions and actions, and then _object-oriented_ programming, which thinks in elements and how they interact--how things are modeled. It's almost like the difference between someone writing a script for an animated movie defining the actions and someone using 3D modeling software to make the animated characters, including facial expressions as one example, based on the descriptions of the characters given by the writer. To make the script work, the designer has to create all the facial expressions in a lifelike manner, define a way for the characters to move to match all of the actions needed (for example, sneaking around is different from running), and make the characters' mouths move in a lifelike fashion to match the words being said.

In short, you can design around what you do (the procedure) or around what you are manipulating (the objects). Generally, Python programs get designed around the objects they manipulate. While you still can code procedurally with Python, the more complicated stuff boils down to objects.

## So what?

Object-oriented programming lets you create (hopefully) efficient systems that can be used in ways beyond the way you currently need. You can create templates that can be used again and again without rewriting the entire codebase. Pretty cool!

## Advanced users: Python is not like Java

Python and Java approach OOP in different ways. A Python project does not _have_ to use classes, as noted above. Python can use procedures to execute. However, Python is, at its core, about objects, even if the developer is working in procedures only.

## Resources

Code examples for this section can be found in [code for objects](../examples/objects.md).

Check out the following resources for more on object-oriented programming and Python.

- [Jeff Knupp on OOP](https://jeffknupp.com/blog/2014/06/18/improve-your-python-python-classes-and-object-oriented-programming/)
- [A Byte of Python on OOP](https://python.swaroopch.com/oop.html)
- [Think Python on OOP](http://greenteapress.com/thinkpython/html/thinkpython018.html#toc182)
- [Dive into Python 3 on objects](http://www.diveintopython3.net/your-first-python-program.html#everythingisanobject)
- [More Dive into Python 3 on objects](http://www.diveintopython3.net/your-first-python-program.html#whatsanobject)
- [The Mozilla Foundation on OOP](https://developer.mozilla.org/en-US/docs/Learn/Drafts/Python/Quickly_Learn_Object_Oriented_Programming)
- [Learn Python the Hard Way on OOP](https://learnpythonthehardway.org/book/ex40.html) *Note: Zed is very anti-Python 3. There are many arguments for Python 3. Please feel free to come discuss that topic with me when you get to it!*
