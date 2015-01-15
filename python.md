part 1

# Basic Syntax
Hey! Now we'll be going over the basic syntax you'll need to use Python. To make this a bit easier, we'll provide the Javascript equivalent as well.

## Variable Declaration
Python is completely object oriented. You do not need to declare variables before using them, or to declare their type. Every variable in Python is an object, thankfully. Also python interprets and declares variable for you when you set them equal to a value.

This section will go over a few basic types of variables: Numbers &  Strings.

###Math Operators
Assume variable a holds 10 and variable b holds 20, then:

|Operator |Description |Example |
|:------------:|:--------------:|:--------------:|
|+|	Addition - Adds values on either side of the operator	|a + b will give 30
|-|	Subtraction - Subtracts right hand operand from left hand operand|	a - b will give -10
|* |	Multiplication - Multiplies values on either side of the operator	|a * b will give 200
|/|	Division - Divides left hand operand by right hand operand|	b / a will give 2
|%|	Modulus - Divides left hand operand by right hand operand and returns remainder	|b % a will give 0
|**|	Exponent - Performs exponential (power) calculation on operators|	a**b will give 10 to the power 20
|//|	Floor Division - The division of operands where the result is the quotient in which the digits after the decimal point are removed.|	9//2 is equal to 4 and 9.0//2.0 is equal to 4.0


### Numbers
To define an integer, use the following syntax:

- myint = 7

### Strings
Strings are defined either with a single quote or a double quotes. Example:
- mystring = 'hello'
- mystring = "bye"

Here are a few examples:
- pen = 10
- pen_in_a_desk = 3
- students = 5

You get the point. Also, variables can not be numbers. So 7 = var, isn't valid.

Also an easier way to remember this is variables appear on the left of the equal sign and values appear on the right side.

## Printing
You'll use print() a whole lot in the future. All it does is output whatever is inside the parentheses.

Print is a function that we will go into later, but just understand that it can take a value. On the first line, we provide a string value "My first Python code!", which is a string because of the quotes. So, you just told Python to output that string to the console. Python completes that task and moves onto the next line where it prints out a different string.

Using the variables from the last section, you'll learn how to print strings:

- print(pen)
- print(pen_in_a_desk)
- print(students)

## Comments

To make a multiline comment type " ''' ".  
If you're using a text editor, make comments by entering '#' before the line of code. To comment multiple lines of code highlight the lines hold CTRL then press the '/' code.

## Excercises

1. Write a program that asks the user to type in a string, and then tells the user how long that string was.

part 2

# tutorial
Standard Data Types:
The data stored in memory can be of many types. For example, a person’s age is stored as a numeric value and his or her address is stored as alphanumeric characters. Python has various standard types that are used to define the operations possible on them and the storage method for each of them.
Python has five standard data types:

1. Numbers
2. String
3. List
4. Tuple
5. Dictionary

Python Numbers:
Number data types store numeric values. They are immutable data types which means that changing the value of a number data type results in a newly allocated object.

Number objects are created when you assign a value to them. For example:

`var1 = 1`
`var2 = 10`
You can also delete the reference to a number object by using the del statement. The syntax of the del statement is:

`del var1[,var2[,var3[….,varN]]]]`
You can delete a single object or multiple objects by using the del statement. For example:

`del var
del var_a, var_b`
Python supports four different numerical types:

1. int (signed integers)

2. long (long integers [can also be represented in octal and       hexadecimal])

3. float (floating point real values)

4. complex (complex numbers)

Examples:
Here are some examples of numbers:

|int   | long           | float     | complex|
|-----:|---------------:|----------:|--------:|
|10    |51924361L       | 0.0       | 3.14j   |
|100   |-0x19323L       |15.20      |45.j     |
|-786  | 0122L          | -21.9     |9.322e-36j|
|080   |0xDEFABCECBDAECB|32.3+e18   | .876j   |
|-0490 |535633629843L   | -90.      |-.6545+0J|
|-0x260 | -052318172735L| -32.54e100| 3e+26J  |
|0x69   |-4721885298529L|70.2-E12   |4.53e-7j

Python allows you to use a lowercase L with long, but it is recommended that you use only an uppercase L to avoid confusion with the number 1. Python displays long integers with an uppercase L.

A complex number consists of an ordered pair of real floating-point numbers denoted by a + bj, where a is the real part and b is the imaginary part of the complex number.

Python Strings:
Strings in Python are identified as a contiguous set of characters in between quotation marks. Python allows for either pairs of single or double quotes. Subsets of strings can be taken using the slice operator ( [ ] and [ : ] ) with indexes starting at 0 in the beginning of the string and working their way from -1 at the end.

The plus ( + ) sign is the string concatenation operator and the asterisk ( * ) is the repetition operator. For example:
```python
!/usr/bin/python

str = ‘Hello World!’

print str # Prints complete string
print str[0] # Prints first character of the string
print str[2:5] # Prints characters starting from 3rd to 5th
print str[2:] # Prints string starting from 3rd character
print str * 2 # Prints string two times
print str + “TEST” # Prints concatenated string
```
This will produce the following result:
```python
Hello World!
H
llo
llo World!
Hello World!Hello World!
Hello World!TEST
```
Python Lists:
Lists are the most versatile of Python’s compound data types. A list contains items separated by commas and enclosed within square brackets ([]). Python doesn't have a native array data structure, but it has the list which is much more general and can be used as a multidimensional array quite easily.

The values stored in a list can be accessed using the slice operator ( [ ] and [ : ] ) with indexes starting at 0 in the beginning of the list and working their way to end -1. The plus ( + ) sign is the list concatenation operator, and the asterisk ( * ) is the repetition operator. For example:

!/usr/bin/python
```python
list = [ ‘abcd’, 786 , 2.23, ‘john’, 70.2 ]
tinylist = [123, ‘john’]

print list # Prints complete list
print list[0] # Prints first element of the list
print list[1:3] # Prints elements starting from 2nd till 3rd
print list[2:] # Prints elements starting from 3rd element
print tinylist * 2 # Prints list two times
print list + tinylist # Prints concatenated lists
This will produce the following result:

[‘abcd’, 786, 2.23, ‘john’, 70.200000000000003]
abcd
[786, 2.23]
[2.23, ‘john’, 70.200000000000003]
[123, ‘john’, 123, ‘john’]
[‘abcd’, 786, 2.23, ‘john’, 70.200000000000003, 123, ‘john’]
```
Python Tuples:
A tuple is another sequence data type that is similar to the list. A tuple consists of a number of values separated by commas. Unlike lists, however, tuples are enclosed within parentheses.

The main differences between lists and tuples are: Lists are enclosed in brackets ( [ ] ) and their elements and size can be changed, while tuples are enclosed in parentheses ( ( ) ) and cannot be updated. Tuples can be thought of as read-only lists. For example:

!/usr/bin/python
```python
tuple = ( ‘abcd’, 786 , 2.23, ‘john’, 70.2 )
tinytuple = (123, ‘john’)

print tuple # Prints complete list
print tuple[0] # Prints first element of the list
print tuple[1:3] # Prints elements starting from 2nd till 3rd
print tuple[2:] # Prints elements starting from 3rd element
print tinytuple * 2 # Prints list two times
print tuple + tinytuple # Prints concatenated lists
This will produce the following result:

(‘abcd’, 786, 2.23, ‘john’, 70.200000000000003)
abcd
(786, 2.23)
(2.23, ‘john’, 70.200000000000003)
(123, ‘john’, 123, ‘john’)
(‘abcd’, 786, 2.23, ‘john’, 70.200000000000003, 123, ‘john’)
```
Following is invalid with tuple, because we attempted to update a tuple, which is not allowed. Similar case is possible with lists:

!/usr/bin/python
```python
tuple = ( ‘abcd’, 786 , 2.23, ‘john’, 70.2 )
list = [ ‘abcd’, 786 , 2.23, ‘john’, 70.2 ]
tuple[2] = 1000 # Invalid syntax with tuple
list[2] = 1000 # Valid syntax with list
```
Python Dictionary:
Python’s dictionaries are kind of hash table type. They work like associative arrays or hashes found in Perl and consist of key-value pairs. A dictionary key can be almost any Python type, but are usually numbers or strings. Values, on the other hand, can be any arbitrary Python object.

Dictionaries are enclosed by curly braces ( { } ) and values can be assigned and accessed using square braces ( [] ). For example:

!/usr/bin/python
```python
dict = {}
  dict[‘one’] = “This is one”
  dict[2] = “This is two”

  tinydict = {‘name’: ‘john’,’code’:6734, ‘dept’: ‘sales’}

  print dict[‘one’] # Prints value for ‘one’ key
  print dict[2] # Prints value for 2 key
  print tinydict # Prints complete dictionary
  print tinydict.keys() # Prints all the keys
  print tinydict.values() # Prints all the values
  ```
  This will produce the following result:

  This is one
  This is two
  ```python
  {‘dept’: ‘sales’, ‘code’: 6734, ‘name’: ‘john’}
  [‘dept’, ‘code’, ‘name’]
  [‘sales’, 6734, ‘john’]
  ```
  Dictionaries have no concept of order among elements. It is incorrect to say that the elements are “out of order”; they are simply unordered.

  Data Type Conversion:
  Sometimes, you may need to perform conversions between the built-in types. To convert between types, you simply use the type name as a function.

  There are several built-in functions to perform conversion from one data type to another. These functions return a new object representing the converted value.
  a long integer. base specifies the base if x is a string.

  Data manipulation
  string methods
  len()
  lower()
  upper()
  str()
  str(x)
  List Method
  list
  list.append(x)
  Add an item to the end of the list; equivalent to    a[len(a):] = [x].
  list.extend(L)
  list.insert(i, x)
  list.remove(x)
  list.pop([i])
  list.index(x)
  list.count(x)
  list.sort(cmp=None, key=None, reverse=False)
  list.reverse()


  An example that uses most of the list methods:
  ```python
  >>>
  >>> a = [66.25, 333, 333, 1, 1234.5]
  >>> print a.count(333), a.count(66.25), a.count('x')
  2 1 0
  >>> a.insert(2, -1)
  >>> a.append(333)
  >>> a
  [66.25, 333, -1, 333, 1, 1234.5, 333]
  >>> a.index(333)
  1
  >>> a.remove(333)
  >>> a
  [66.25, -1, 333, 1, 1234.5, 333]
  >>> a.reverse()
  >>> a
  [333, 1234.5, 1, 333, -1, 66.25]
  >>> a.sort()
  >>> a
  [-1, 1, 66.25, 333, 333, 1234.5]
  >>> a.pop()
  1234.5
  >>> a
  [-1, 1, 66.25, 333, 333]
  ```python


  part 3

  #Control Flow



  ##Conditional Operators

  ###What is an Operator?

  Simple answer can be given using expression 4 + 5 is equal to 9. Here, 4 and 5 are called operands and + is called operator. Python language supports the following types of operators.

  ###Math Operators

  Assume variable a holds 10 and variable b holds 20, then:

  |Operator |Description |Example |
  |:------------:|:--------------:|:--------------:|
  |+|	Addition - Adds values on either side of the operator	|a + b will give 30
  |-|	Subtraction - Subtracts right hand operand from left hand operand|	a - b will give -10
  |* |	Multiplication - Multiplies values on either side of the operator	|a * b will give 200
  |/|	Division - Divides left hand operand by right hand operand|	b / a will give 2
  |%|	Modulus - Divides left hand operand by right hand operand and returns remainder	|b % a will give 0
  |**|	Exponent - Performs exponential (power) calculation on operators|	a**b will give 10 to the power 20
  |//|	Floor Division - The division of operands where the result is the quotient in which the digits after the decimal point are removed.|	9//2 is equal to 4 and 9.0//2.0 is equal to 4.0

  ###Comparison Operators

  Assume variable a holds 10 and variable b holds 20, then:

  |Operator |Description |Example |
  |:------------:|:--------------:|:--------------:|
  |==	|Checks if the value of two operands are equal or not, if yes then condition becomes true.|	(a == b) is not true.
  |!=|	Checks if the value of two operands are equal or not, if values are not equal then condition becomes true.|	(a != b) is true.
  |<>|	Checks if the value of two operands are equal or not, if values are not equal then condition becomes true.|	(a <> b) is true. This is similar to != operator.
  |>|	Checks if the value of left operand is greater than the value of right operand, if yes then condition becomes true.	|(a > b) is not true.
  |<	|Checks if the value of left operand is less than the value of right operand, if yes then condition becomes true.	|(a < b) is true.
  |>=|	Checks if the value of left operand is greater than or equal to the value of right operand, if yes then condition becomes true.|	(a >= b) is not true.
  |<=|	Checks if the value of left operand is less than or equal to the value of right operand, if yes then condition becomes true.|	(a <= b) is true.

  ###Assignment Operators

  Assume variable a holds 10 and variable b holds 20, then:

  |Operator |Description |Example |
  |:------------:|:--------------:|:--------------:|
  |=|	Simple assignment operator, Assigns values from right side operands to left side operand|	c = a + b will assigne value of a + b into c
  |+=|	Add AND assignment operator, It adds right operand to the left operand and assign the result to left operand|	c += a is equivalent to c = c + a
  |-=|	Subtract AND assignment operator, It subtracts right operand from the left operand and assign the result to left operand|	c -= a is equivalent to c = c - a
  |*=|	Multiply AND assignment operator, It multiplies right operand with the left operand and assign the result to left operand	|c *= a is equivalent to c = c * a
  |/=|	Divide AND assignment operator, It divides left operand with the right operand and assign the result to left operand|	c /= a is equivalent to c = c / a
  |%=|	Modulus AND assignment operator, It takes modulus using two operands and assign the result to left operand|	c %= a is equivalent to c = c % a
  |**=|	Exponent AND assignment operator, Performs exponential (power) calculation on operators and assign value to the left operand	|c **= a is equivalent to c = c ** a
  |//=|	Floor Dividion and assigns a value, Performs floor division on operators and assign value to the left operand	|c //= a is equivalent to c = c // a

  ###Bitwise Operators

  Bitwise operator works on bits and perform bit by bit operation. Assume if a = 60; and b = 13; Now in binary format they will be as follows:

  |Operator |Description |Example |
  |:------------:|:--------------:|:--------------:|
  |& |	Binary AND Operator copies a bit to the result if it exists in both operands. |	(a & b) will give 12 which is 0000 1100
  | (pipe) |	Binary OR Operator copies a bit if it exists in eather operand. |	(a "pipe" b) will give 61 which is 0011 1101
  |^|	Binary XOR Operator copies the bit if it is set in one operand but not both.|	(a ^ b) will give 49 which is 0011 0001|
  |~|	Binary Ones Complement Operator is unary and has the efect of 'flipping' bits.|	(~a ) will give -61 which is 1100 0011 in 2's complement form due to a signed binary number.|
  |<<|	Binary Left Shift Operator. The left operands value is moved left by the number of bits specified by the right operand.|	a << 2 will give 240 which is 1111 0000
  |>>	|Binary Right Shift Operator. The left operands value is moved right by the number of bits specified by the right operand.|	a >> 2 will give 15 which is 0000 1111|

  ###Operator Precedence
  |Operator |Description |
  |:------------:|:--------------:|
  |**|	Exponentiation (raise to the power)
  |~ + -|	Ccomplement, unary plus and minus (method names for the last two are +@ and -@)
  |* / % //|	Multiply, divide, modulo and floor division
  |+ -|	Addition and subtraction
  |>> <<|	Right and left bitwise shift
  |&|	Bitwise 'AND'
  |^ (pipe)|	Bitwise exclusive `OR' and regular `OR'
  |<= < > >=|	Comparison operators
  |<> == !=|	Equality operators
  |= %= /= //= -= += *= **=|	Assignment operators
  |is is not|	Identity operators
  |in not in|	Membership operators
  |not or and|	Logical operators

  ##IF Statement

  The **_if_** statement of Python is similar to that of other languages. The if statement contains a logical expression using which data is compared and a decision is made based on the result of the comparison.

  Some important pieces of all these statements is that colons and indention are key in Python. You must indent after the colon for it to read the statement. if you do not then it will not be included in the statement. It is as if you are starting a new line or expression.

  SYNTAX:
  ```python
  if expression:
  statement(s)
  ```

  EXAMPLE:
  ```python
  var1 = 100
  if var1:
  print "1 - Got a true expression value"
  print var1

  var2 = 0
  if var2:
  print "2 - Got a true expression value"
  print var2
  print "Good bye!"
  ```
  RESULT:
  ```
  1 - Got a true expression value
  100
  Good bye!
  ```

  ##IF ELSE Statement

  An **_else_** statement can be combined with an if statement. An else statement contains the block of code that executes if the conditional expression in the if statement resolves to 0 or a false value.

  The else statement is an optional statement and there could be at most only one else statement following if.


  SYNTAX:
  ```python
  if expression:
  statement(s)
  else:
  statement(s)
  ```

  EXAMPLE:
  ```python
  var1 = 100
  if var1:
  print "1 - Got a true expression value"
  print var1
  else:
  print "1 - Got a false expression value"
  print var1

  var2 = 0
  if var2:
  print "2 - Got a true expression value"
  print var2
  else:
  print "2 - Got a false expression value"
  print var2

  print "Good bye!"
  ```

  RESULT:
  ```
  1 - Got a true expression value
  100
  2 - Got a false expression value
  0
  Good bye!
  ```

  ##ELIF

  The **_elif_** statement allows you to check multiple expressions for truth value and execute a block of code as soon as one of the conditions evaluates to true.

  Like the else, the elif statement is optional. However, unlike else, for which there can be at most one statement, there can be an arbitrary number of elif statements following an if.

  Key Javascript and Ruby differences:

  - notice the difference in how the else if syntax is different from both ruby and javascript.

  - there is also the need for the colon at the end of each expression and indention of the statement.

  SYNTAX:
  ```python
  if expression1:
  statement(s)
  elif expression2:
  statement(s)
  elif expression3:
  statement(s)
  else:
  statement(s)
  ```

  EXAMPLE:
  ```python
  var = 100
  if var == 200:
  print "1 - Got a true expression value"
  print var
  elif var == 150:
  print "2 - Got a true expression value"
  print var
  elif var == 100:
  print "3 - Got a true expression value"
  print var
  else:
  print "4 - Got a false expression value"
  print var

  print "Good bye!"
  ```

  RESULT:
  ```
  3 - Got a true expression value
  100
  Good bye!

  ```



  ##While Statement

  A **_while_** loop statement in Python programming language repeatedly executes a target statement as long as a given condition is true.

  SYNTAX:
  ```python
  while expression:
  statement(s)
  ```

  EXAMPLE:
  ```python
  count = 0
  while (count < 9):
  print 'The count is:', count
  count = count + 1

  print "Good bye!"
  ```

  RESULT:
  ```
  The count is: 0
  The count is: 1
  The count is: 2
  The count is: 3
  The count is: 4
  The count is: 5
  The count is: 6
  The count is: 7
  The count is: 8
  Good bye!
  ```

  ##ELSE Statement with WHILE Statement

  Python supports to have an else statement associated with a loop statement.

  1. If the else statement is used with a for loop, the else statement is executed when the loop has exhausted iterating the list.

  2. If the else statement is used with a while loop, the else statement is executed when the condition becomes false.

  SYNTAX:
  ```python
  while expression:
  statement(s)
  else expression:
  statement(s)
  ```

  EXAMPLE:
  ```python
  count = 0
  while count < 5:
  print count, " is  less than 5"
  count = count + 1
  else:
  print count, " is not less than 5"
  ```

  RESULT:
  ```
  0 is less than 5
  1 is less than 5
  2 is less than 5
  3 is less than 5
  4 is less than 5
  5 is not less than 5
  ```

  ##FOR Statement

  The **_for_** loop in Python has the ability to iterate over the items of any sequence, such as a list or a string.

  SYNTAX:
  ```python
  for iterating_var in sequence:
  statements(s)
  ```

  EXAMPLE:
  ```python
  for letter in 'Python':     # First Example
  print 'Current Letter :', letter

  fruits = ['banana', 'apple',  'mango']
  for fruit in fruits:        # Second Example
  print 'Current fruit :', fruit

  print "Good bye!"
  ```

  RESULT:
  ```
  Current Letter : P
  Current Letter : y
  Current Letter : t
  Current Letter : h
  Current Letter : o
  Current Letter : n
  Current fruit : banana
  Current fruit : apple
  Current fruit : mango
  Good bye!
  ```

  You can also iterate through an array. len() is a built in function that is finding the length of the array and the range() is giving the expression a number range to iterate through.

  EXAMPLE:
  ```python
  fruits = ['banana', 'apple',  'mango']
  for index in range(len(fruits)):
  print 'Current fruit :', fruits[index]

  print "Good bye!"
  ```

  RESULT:
  ```
  Current fruit : banana
  Current fruit : apple
  Current fruit : mango
  Good bye!
  ```




  ##Assessment

  ``Create an example that illustrates the combination of``
  ``an else statement with a for statement that searches``
  ``for prime numbers from 10 through 20.``


  part 4


  # Function Syntax and Scope

  Functions are extremely powerful and essential to any useful code. It's easiest to think of functions in python like functions in math. They are first called, usually taking in some values, form operation

  ## Function Basics

  Functions in Python are very much like functions in ruby. Here is the basic syntax

  ``` python
  def hello():
    print "Hello, World!"

    hello()
    ```

    If you come from ruby, you'll probably recognize the `def` keyword, which stands for define, followed by the function name. The `def` indicates the start of a function declaration. The name of the function is then followed by parenthesis and a colon. Remember that python uses rigid rules on indents, so anything after the colon that is tabbed will be apart of the function being made.

    For ruby users, notice that the parenthesis are needed, so you cannot leave them off if you are not using them. Also note that there is no `do` and `end` syntax.  Python recognizes the beginning of the function body using the colon and the end using line indents.

    In order to use the function, you must call the function. This is represented by simply entering in the name of the function with parenthesis: `hello()`.

    ##Parameters and Arguments

    Functions wouldn't be all that useful unless your able to pass things to them. Heres is what this concepts look like

    ``` python
    def printStr(str):
      print str;

      printStr("Hello, World!")
      ```
      First lets discuss the terms. An argument is what is passed into the function. In this case, that would be `"Hello, World!"`. While a parameter is the variable that is declared with the function. In this case, that would be `str`.

      This syntax is exactly like most other languages, including ruby.

      ##Returning
      All the function we have been using is doing so far is printing a string. Most of the time, this is not very useful. A function in mathematics takes arguments, does some operation, and then returns a new value. Now lets look at how we return values python.

      ``` python
      def add(num1,num2):
        return num1 + num2

        print add(1,2)
        ```
        Notice that the print statement is no longer in the function, but instead is called on the function call itself. This is because the function is returning the value, not printing it. You can think about it as the function call is being replaced with the value that is being returned, in which we are then printing to the terminal.

        This is very similar to the return statement in both JavaScript and Ruby and probably most other languages.

        ##Functions in Functions so your function can function

        One thing to note about Python is that is allows you to call functions within functions.

        ``` python
        def add():
        return addMore()
        def addMore():
        return 1
        print add()
        ```
        `addMore()`is called within the other function `add()`. If you come from JS or Ruby, this is very familiar.

        ## Scope

        Scope is a difficult and abstract concept for a lot of people to understand. Python has strict scoping  guidelines that can be broken into two different rules. When looking for a variable name, python essentially looks in two places.

        1. The local namespace, or scope.
        2. The global scope.

        The local scope is any variable that is declared within the given function. The global scope is any variable that is declared outside of any function or class. It always does it in this order, so the local variable will always be used over the global variable.

        Lets do some examples

        ``` python
        n = 1
        def add():
        return n + 1
        print add()
        ```
        This code will not break the program. Python first checks for `n` in the local function, which it can't find, and then looks for it in the global scope, where it is declared.
        ``` python
        def add():
        n = 1
        return n + 1
        print add()
        print n
        ```
        This code will break the program. The last line, `print(n)`, looks for n in the local scope, which is the global scope, and the global scope, which is the same as before, and cannot find the variable declaration. In short, any variable declared within a function or loop is immediately "destroyed" one the function or loop ends.

        One more example that is important is that the local scope only specifies the current function's scope, and not any "outer" scopes that may be in play. Lets look at a slightly different example from above:
        ``` python
        def add():
        n = 1
        return addMore()
        def addMore():
        return n + 1
        print add()
        ```
        Intuitively, this program looks like it would work. Since the `addMore()` function is called in the `add()` function, you would think that `n` could be used. This is, in fact, false. The local scope only includes what is in the current function, and not in any function that it may be nested in.

        ##Quirks
        One thing to be careful of when your sending in arguments into a function is that you can change them with mutator methods. For example, appending an element onto a list.
        ``` python
        arr = [1,2]
        def change(array):
        array.append(3)
        print array
        change(arr)
        print arr
        ```
        In this function, a list is sent in as a argument, and the related parameter is appended to. The original `arr` is changed to `[1,2,3]`, even outside of the function.

        Another thing to note is when you assign a variable name in a function, it overides the global variable while inside that function.

        ``` python
        num = 2
        def change():
        num = 3
        print num
        change()
        print num
        ```
        Inside the function, `num` is 3 and outside `num` is still 2. The function created a local variable called `num`.

        One last thing to note is that Python will create the local variable before is reads what it is being assigned to. From the last example, this will throw an error.

        ``` python
        num = 2
        def change():
        num = num + 3
        print num
        change()
        print num
        ```
        The functions initializes the local variable `num` and before assigning it anything tries to assign it itself. It causes an error. To fix this, all you do is have to add a buffer variable.

        ``` python
        num = 2
        def change():
        num_alt = num
        num = num_alt + 3
        print num
        change()
        print num
        ```
        This will work fine.


        ##Built-in Functions
        Python has a plethora of built-in functions that it allows you to use. To use them, its as simple as calling a function that you made yourself. Here is an example:
        ``` python
        print abs(-42)
        ```
        `abs()` is a built-in python function that returns the absolute value of the given number. As expected, this program would print `42`.

        Here is just a few of the many Python built-in functions
        * `abs()`
        * `min()`
        * `max()`
        * `any()`
        * `filter()`
        * `map()`

        ##Importing Functions

        Ever wonder where all of the built-in functions are coming from? They're essentially coming from files that declare python functions the same way we did above. You can actually make your own functions and import them into other documents to use functions you write. This is how libraries are created and used. For example, Python has a math module (or library) that we can use. We need to, however, import it first.

        ``` python
        import math

        print math.sqrt(16)
        ```
        `math` is the name the module that you are importing, or the name of the file that you want to use methods from. When using one of these methods, you then have to write `module.function()` in order to use them. Math has a variety of very useful functions that you will undoubtedly need if you keep working with python.

        This is very similar to Ruby's `require` keyword.

        ## Putting it All Together

        1. Create a function that takes in a list and returns a random item from that list (hint: look up the random module)
        2. Create a function with a hard-coded list that calls the function above and returns a random item from the local hard-coded list.


part 5

#Classes and Object Oriented Programming

Classes are an important part of python, it allows us to create objects and manipulate them through methods to reach our goals.


----------

##Creating a class

Creating a class is simple, all it requires is one line of code.
``` python
class Example(object):
```
With our class we created, we can begin to input an object.

----------


##Initialize your object

One initialize command will allow you to create new objects.
``` python
def __init__(self, param1, param2, param3):
  self.param1 = param1
  self.param2 = param2
  self.param3 = param3
  ```
  Here `param` is equivalent to any parameters that you wish to add.

  This is how we initialize an object to be manipulated by further methods.

  ----------

  ##Creating your object

  Now that we can initialize the object, it's time to make one. Let's give it a variable.
  ``` python
  class Example(object):
    def __init__(path, params):
      pass
      var = Example(params)
      ```
      It is important to note that your variable name will become the `path` so any parameters are entered afterwards.

      ----------


      ##Scope

      Its important to note not all variables may work in your class. This is determined by where the variables are located.
      ``` python
      xkcd = "antigravity"
      class Example(object):
      marbles = "marble"
      def __init__(self, param1):
      self.param1 = param1
      def method(self):
      print xkcd
      print marbles
      print self.param1

      test = Example("text!")
      test.method()
      ```
      In this scenario, the variable `xkcd` is outside of the class. It is a global variable and can be used anywhere in the code. On the other hand, the variable `marbles` is declared inside the class. It is a member variable and can only be called inside the class itself. Finally we have `self.param1` which is an instance variable. We can only call it inside of the method because we called `self` as a parameter.

      Understanding scope is extremely important and can stop many problems that arise due to improperly called variables.


      ----------


      ##Methods

      Methods are what makes classes useful. They are the means of manipulating the data we have stored in our class. As seen above methods are similar to functions just called upon our classes. They are limited to only the classes that they reside in so unlike other methods such as `.len()` and `.str()` they will not work on anything that isn't the class they correspond to.

      A method is created by:
      ``` python
      def method(self):
      # Rest of the code
      ```
      The method is called by using:
      ``` python
      randomname.method(param)
      #param if you have one set otherwise it can be left empty.
      ```

      Methods can be treated the same way as functions as they perform a very similar function the only main difference being the restrictions on the usage of methods and the way they are implemented. It is important to note that functions can be used on objects, however functions are often less relied on due to their inability to access information locally to the object.


      ----------


      ##Inheritance

      Classes can be called in the creating of another class to inherit that classes properties,

      ``` python
      class Example(object):
      def __init___(self):
      # blah blah blah coding blah
      def method(self):
      print "stuff"

      class NextExample(Example):
      def post_history(self):
      print "Other Stuff"
      ```
      By calling the previous class in the new class, the new class inherits the objects of the previous class and can thus act on them in a independent environment that will no longer affect other objects in the previous class.

      Additionally, a inherited class can override the previous class by naming the method the same as before.

      ``` python
      class Example(object):
      def __init___(self):
      # blah blah blah coding blah
      def method(self):
      print "stuff"

      class NextExample(Example):
      def method(self):
      print "OVERRIDE!"
      ```
      Doing so will override the object in the `NextExample` class without affecting objects in the `Example` class. This is useful in ensuring a common method can create different results depending on circumstance.


      ----------

      ##Assessment

      Create a class and a inherited class and have them print out a different statement for the same method for two different objects.

        
