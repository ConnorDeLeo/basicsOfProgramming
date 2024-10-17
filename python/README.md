# Python Basics

## File type
I'm sure you know what a file type is, so Python's is `*.py`, when you make a new file in VSC, you need to type in the file extension yourself (as it supports many languages and file types) so don't forget the `.py`!

## Syntax
Syntax is the way you structure a program, like grammar. *Most* languages use a standard with tabs (or spaces for weird people), semi-colons, and brackets. To simplify things, Python throws the brackets and semi-colons out the window! Brackets are replaced by a single colon, we'll get to that later. Variable nomenclature is also a part of syntax! I use Camel Case (`likeThisStatementIs` or `this`), but there is also Snake Case (`like_this_one` or `this`), standard lowercase (`dontusethisone`), etc.

## Comments
The most important piece of your code is comments. Most people don't want to read through your jumbled spaghetti to figure out what your deprecated function from seven years ago does, and neither do you! To make comments in Python use the `#` operator while using `'''` on two lines can create multiline comments. Heres an example:
```python
# This is a comment
#thisisalsoacommentbutdontdothis

print("Comments!") # Comments can also be used at the end of a line

'''
This is a multiline comment
You can write paragraphs in these
'''
```

Although you can use comments at the end of a line, they should (in my opinion) only be used for simple notes (like expected values) while a full line should be dedicated to a **short** function/method description. Multiline comments should be used for blocking out large chunks of code for debugging, describing the overall code, or writing attributes.

## Datatypes
Think of a number, you probably think of an `integer` like `1, 2, 3`, but thats not the only datatype. You also have characters (denoted by `char`) like `'a', 'b', 'c'`, strings (denoted by `str`) like `"Hello!"` (note the difference in `'` for a `char` vs `"` for a `str`), booleans (denoted by `bool`) which is a `1` or a `0` (in Python's case its `True` or `False`), and floating point values (stuff with decimals denoted as `float`) like `1.23, 4.56, 7.891011` (note how there is no symbolism around numbers as there is with text). In programming, giving a variable (dataholder) a value is called setting or initializing, in *most* languages you need to denote what datatype you're using, but you don't need to say it explicitly in Python. Sometimes you'll need to cast one datatype to another (most commonly on inputs), and you'll just need to take the datatype you want, and "multiply" by the variable you're attempting to change (`(int)x`). Heres an example of setting and casting different variables:
```python
# Setting
intOne = 1
intTwo = 1000

floatOne = 1.01
floatTwo = 1.0001

boolOne = True
boolTwo = False

charOne = 'a'
charTwo = 'b'

strOne = "One"
strTwo = "Two"

# Casting
strThree = "1"
intThree = (int)strThree
```

## Functions
The basic methods used to run programs in Python are prewritten (they're already a part of your Python installation), although you can write your own for more advanced stuff. Most functions take arguments, the inputs to the function like `x` in `f(x)`. These can be any datatype, but certain functions take certain datatypes (i.e. a function that rounds a float point number won't take a string). The variables used as arguments don't have to be previously defined, they can be set the moment you "call" that function! Here are some examples:
```python
# This pulls in a library of functions, we'll cover that later but I thought it should be here
import math

# Variable declaration
floatOne = 1.01
strOne = "One"

# Ceiling function (rounds a floating point value up to the nearest integer), math is the library so the function ceil is called from math via the `.`
roundedOne = math.ceil(floatOne)
roundedTwo = math.ceil(1.001)
 
# Print function (sends a message output to the console, arguably the most important function)
print(strOne)
print("Two")
```

## Math
Math works like it does on paper, except operators can be a bit odd. For addition, subtraction, multiplication, and division use `+,-,*,/` respectively. Some symbols must come from a library (like the math one used above, that one contains lots of things like square roots, trig functions, etc.). The weird stuff (in my opinion) comes from parentheses. Use an overly large amount of parentheses so you can easily debug and leave nothing up to chance, I'll give examples below. Exponentials are also odd as they are denoted by `**`. Here are examples:
```python
import math

addition = 1 + 2 # addition is equal to 3
subtraction = 2 - 1 # subtraction is equal to 1
multiplication = 2 * 2 # multiplication is equal to 4
division = 4 / 2 # division is equal to 2
exponent = 2**3 # exponent is equal to 8

parentheses = 2 + ((4 - 1) * (3**2)) # parentheses is equal to 29

sinOne = math.sin(1) # sinOne is approx. 0.841 (Python does math in radians)
```

## Inputs
You want a program that doesn't do the exact same thing every time you run it? Thats inputs baby! Using the `input()` function set to a variable, the user can type a value into the console and Python knows what to do with it! Lets look at an example:
```python
userIn = input() # userIn equals what the user types

# lets assume they type 1234 and output that with a print() statement
print(userIn) # outputs 1234 to the console
```

## Assignments
Head over to the `/assignments` directory, I'll give you new ones when you need them!