[Back to the index](/BeginnerCodersWWCATX)

# Using Errors to Fix Your Code

_A Primer for Women Who Code ATX_

## Errors in Python

As a feature of its design, Python does not let errors pass silently. That means
that whenever the Python interpreter encounters an error, it will tell you and
stop trying to run the code. This feature can be very useful for the beginner
who wants to understand their code.

## The stack trace

When your code raises an error, the interpreter (in your terminal) displays a
_stack trace_. In Python, only one error gets raised at a time, so seeing only
one error does _not_ mean your code only has one error!

Note that some people might call this a _traceback_ after the way it is
presented in the terminal. The two terms are equivalent; both are actually
shorter forms of _stack traceback_. In fact, the module that generates the stack
traceback is called `traceback`, which is what you will see in the interpreter.

Want to see one? Check out the [errors Juypter notebook](https://nbviewer.jupyter.org/github/nimbinatus/BeginnerCodersWWCATX/blob/gh-pages/examples/errors.ipynb)
for the input and output of some code.

## Troubleshooting your code

You can use the stack trace to work your way back through your code to figure
out how it works. We are not going to go heavily into debugging in this
discussion, but we can talk a bit about the basics of using the stack trace to
understand your code and why it failed.

First, use the stack trace to figure out where this problem lies. In a simple
script that never references other scripts, the stack trace shows the line that
has a problem and a caret (`^`) where the error seems to occur to the
interpreter. Don't rely on the caret to show you where to fix it, however. If
the interpreter is having trouble running that line, the caret may just be at
the end of the line to indicate a general problem. Also, the line itself may not
be the correct line if the "thought" of the code continues (for example, a `for`
loop that continues on multiple lines may raise the error at the beginning of
the second iteration of the loop, but the problem might be three lines in).

In scripts that reference other scripts, the stack trace may show a path the
interpreter took through multiple files to the error itself. The last line is
the one you're looking for.

The error code itself may not be the most helpful, but the text afterward often
provides more information. For example, the following error itself may be a bit
cryptic, but the informational text afterwards provides just enough context to
understand where things are headed:

    NameError: name 'apple' is not defined on line 7

In this example, the variable `apple` was used on line 7 before it was defined
in the code. To fix this error, you need to define `apple` before line 7.

## Python Koans

A great way to learn more about errors and stack traces _and_ learn Python at
the same time is to run the Python Koans.

Install them through
[this handy dandy link](https://github.com/gregmalcolm/python_koans).

## Resources

-   [The official docs](https://docs.python.org/3/library/exceptions.html)
-   [A lovely flowchart for errors](http://pythonforbiologists.com/index.php/29-common-beginner-python-errors-on-one-page/)
-   [A great chart of errors if the official docs are too much](https://www.tutorialspoint.com/python/standard_exceptions.htm)
-   [Think Like a Computer Scientist on errors in code](https://interactivepython.org/courselib/static/thinkcspy/Debugging/KnowyourerrorMessages.html)
