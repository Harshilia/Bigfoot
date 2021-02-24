Bigfoot
=======

Bigfoot is a language interpreter like Python, made in Python.

The project contains:

- Lexer based on Regex
- Recursive Parser
- Interpreter with AST-walking
- REPL functionality

Bigfoot doesn't require any third-party libraries.

However, Bigfoot still uses the standard Python compiler until I can figure out how to make one myself :)

What the language looks like:

.. code-block::

    func map(arr, fn):
        r = []
        for val in arr:
            r = r + [fn(val)]
        r

    func factorial(n):
        if n <= 1:
            1
        else:
            n * factorial(n - 1)

    print(map(1...10, factorial))


You can find more examples in ``tests`` directory.

How to try it:

.. code-block::
    
    git clone https://github.com/Harshilia/Bigfoot.git
    cd Bigfoot
    python -m Bigfoot tests/factorial.bgf
