Snippetest
==========

This tool is a set of gedit snippets for python. The goal of help and speed up
the development, mostly using BDD approach.

I strongly recommend the you install the [gmate](http://github.com/gmate/gmate)
and the package gedit-plugins.

Smart def
---------

The Smart def snippet speeds up the method definition. The activation is made
with **Ctrl + u**. The examples below show the ways to use:

Type the line below and press Ctrl + u with the cursor on the line

    it should return the sum of two numbers

and you will have this (the | represents the cursor):

    def it_should_return_the_sum_of_two_numbers(self):
        |

You can pass params too:

    it should return the sum of two numbers(number1, number2)

And you will have this:

    def it_should_return_the_sum_of_two_numbers(self, number1, number2):
        |

--------------------------------------------------------------------------------

You can also do this...

    def it should return the sum of two numbers

This...

    def             it should return the sum of two numbers

This...

    it should return the sum of two numbers:

This...

    def it should return the sum of two numbers     ():

Or many combinations of fails syntax that you will have this:

    def it_should_return_the_sum_of_two_numbers(self):
        |


Unittest
--------

Type **ut** and then press **Tab** and you get this:

    import unittest
    from should_dsl import *

    class ClassName(unittest.TestCase):
        |

You only have to write the class name and press tab again.

I assume that you use the amazing package [should-dls](http://github.com/hugobr/should-dsl)
that gives you a lot of matchers and turns your test/specs more readable.

