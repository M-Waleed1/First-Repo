
--- 
Escape character
---

\b -->back space(Remove the letter before it)

Escape New line print("Hello \
World")

`\' --> print single quote- same in double quote

\n --> New line (called line feed)\r --> carriage return 

```
print("123456\rabcd")
output: abcd56
explain:
take after "\r" and put first and remove the same number of letters(digits) and complete it
```

\t --> tab(about 5 spaces)\XHH --> letter hex value

```letter in hex\x47 --> O```

>all Escape character use in string

---
**Concatenation**

is a theory of link 2 string together in python use '+'
```
msg = "Welcome"
lang = "Python"
print(msg + lang)
- Space is a character
- Can be at same variable 
 ```
 
---

Var1 = "This"
var2 = 'This'
if you don't need to use escape character to put quotes you can use this way
var3 = "This 'is'" 
OR
var3 = 'This "is"'


>To print a multiple lines we 
>""" string """
>OR
>''' string '''

---
1. Data in python is object
2. object contains elements
3. every element has its own index 
4. python use zero based indexing (start count from 0)
5. use [] to access the elements
6. enable accessing parts of string, tuples and lists 


>I love python
>I = 0> 
>l = 2
>p = 7 


>**can use negative values to get the element from right**######Slicing

```
syntax
var[start:end]
var[start:end:step]
```


----

> **I replace (.) with (-) as give me error in typing**
> Len(variable) or variable-len() 
> Get the length of variable



 Strip --> remove space from start and end 
 Left strip --> remove spaces from left
 Right strip --> remove spaces from right 

>Can use variable-strip('#') to remove # sign from the string
   
   - variable-title() --> make first letter in each word capital and if digit before letter make that letter capital like 2d --> 2D
   
   - capitalize is the same of title difference between them the digit before letter still small 2d --> 2d
   
   - ZFILL() --> pad a string with zeros in left to complete the width you give it `var.zfill(3)
   
   - variable-upper() --> make all letters to capital 
   
   - Variable-lower() --> make all letters to small

| Split                   | Right split                                      |
| ----------------------- | ------------------------------------------------ |
| divide string into list | divide the string into list but start from right |


variable-split("-", 2) 
"-" --> that like (.) divide based on it 
2 --> the number of parts 

>start count from zero 


- variable-center(15, "@")
make a word in center and it length 15 and replace white-spaces with @ sign

- variable-count("PHP",0 ,25)
  give you the number of the text you need to know how many times repeated
  0 --> start search from it
  25 --> end search at it
```swapcase convert capital to small vice verse```
   
   
   - startwith("G")--> true `--> Falsesame to `endwith
   --- 

--- 
variable-index("letter") --> to find the letter and return its place you can use find it's the same

difference:
- error print as -1 in find

can give it ("letter", start, end)

- `rjust, ljust 
  give it width and sign variable-`rjust`(15, "@")
  
- `splitlines()`
  each line put as a value in a list Variable
  
- `expandtabs()` 
  variable-`expandtabs`(2) control the number of spaces in tab

- can use is(word) --> return True or False
  word can be space, lower, capital, identifier, alpha, `alnum`
---
- Replace(old value, new value, count)
  `a = "Hello One Two Three One One"
  `print(a.replace("one", "1", 2))
  
- Join(Iterable)
  `mylist = ['osama', 'mohamed', 'web']`
  `print("-".join(mylist))`
  output:
  `osama-mohamed-web
---
### Old Way to String Formatting 

% --> called place holder
`"my name is %s" % "Osama"`

>for multi place holder write variables in (variable-1, variable-2, etc...)

| place holder | type of data |
| :----------: | :----------: |
|      %s      |    String    |
|      %d      |   Interger   |
|      %f      |    Float     |

>To control the decimal point: 
%.2f --> 2 numbers after decimal point 

**can use %.5s --> first 5 letters** 

----
### New Ways to String Formatting

`print("My name {}".format("variable"))`
variable take index (0) 
u can use index to determine which variable first 
left the arrange first
{1:.2f}.format(1, 2, 3)

| place holder | Type of data |
|:------------:| ------------ |
|     {:s}     | String       |
|     {:d}     | Integer      |
|     {:f}     | Float        |

>Control Decimal point 
>{:.2f} 

**can use {:.5s} --> first 5 letters**

can format strings as
{:-d} --> After 3 numbers will put this sign('-')
**not all sign acceptable**

can use format f"{variable}"

`print(f"My name is: {MyName} /n My age is: {MyAge}")

---
# Strings Finished