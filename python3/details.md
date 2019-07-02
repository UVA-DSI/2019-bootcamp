## Strings
* A string is a 'string' of characters
  * 'apple'  # letters
  * 'blue42' # letters and numbers
  * 'i am the very model of a modern major general' # spaces are fine
  * '7 hills' # it can even start with a number
  
## Comments
We also introduce comments here, the computer will ignore everything after the '#' symbol. There are other forms but we'll see them later on.

## Variables
You can "save" things as variables. For those curious as to what's going on under the hood...in python a variable is actually just a pointer to the location in memory where the object lives.
* a = 'apple'
  * a is the variable
  * = is the assignment operator
  * 'apple' (a string) is the object assigned to a
  
* *Important Note*: the assignment operator is not like an equals sign
  * a=5
  * a=7
    * totally works, a was just reassigned to point to 7
    
## Functions
* print(a) # this function will show us what a points to
* we know that print is a function because there is no space between print and the "("
* format of a function: name(arguments)
* we say we "call" a function
* *this is super important* in python the way to spot a function is no space before a "(" and a letter or number
  * [python built-in functions](https://docs.python.org/3/library/functions.html)
  * print(...)
  * type(...)
  * pow(...)
  * in an equation you may see 5*(2+3), you won't seet 5(2+3) (try it and see what happens)
  
## Indexing
* for objects with an order you can access individual elements
* [indexing](indexing.png)
* you can also pull out slices
  * syntax [X:Y]
    * starting at X
    * upto but not including Y

## Lists
* represented like functions but with [...]
* there is an order to the items
* the items can be of any type

## Dictionary
* represented like lits but with {...}
* there is no order to items
* items contain two pieces: a key and a value represented key:value and the key must be a string

## loops - used when you want to repeat code
* for loop
  * for X in Y: << code >>
    * X is a new variable created on the spot
    * Y is some preexisting iterable
    * << code >> is a block of code you want to repeat
    * eg: for x in range(10): print(x)

* while loop
  * while Z: << code >>
    * Z is a boolean
    * << code >> is a block of code you want to repeat
    * eg: while i<10: print i; i+=1

## if statements
* example
  * if X: << code A >>
  * else: << code B >>
    * X is a boolean
    * << code A >> is some code
    * << code B >> is some code, could be the same
    
