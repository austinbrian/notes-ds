# Python basics
## Python is...
- high level
- open source
- object oriented
- development language
- statistical analysis
- rapid development

(Python is also generally better at integrating with other big data technology.)

## Data Types
Integers - it's a 32bit memory, so it just stores the 32 bits *before* the decimal, and won't round, etc.
    Two consecutive division signs "//" conducts "integer division" on floats - will drop the remainder.

Typecasting = means to pretend, or cast, as if it's another data type

## Slicing
*C-style formatting*
print("value = %f" % 1.0)

*define step size of 2*
s = 'Hello world'
`s[::2]` will yield 'Hlowrd'
If you want to define a source for the step size, do that first. So:
`s[:5:2]` will yield 'Hlo'
object[start:stop:step]


## Dictionaries
Dictionaries are key value pairs
You can just use curly brackets:
``` params = {"parameter1" : 1.0,
              "parameter2" : 2.0,
              "parameter3" : 3.0,}
```
Ask for the value with dict[key]

## Functions
Difference between for loops and while loops:
- *For loops* have you iterate over **every item in sequence**
- *While loops* take a condition, and make changes to a variable **until the condition is satisfied**.
..- (`Break` will end the while loop without satisfying the actual condition, but if another condition is satisfied)

## Notebooks
- **Jupyter notebooks** are useful for breaking down code into little pieces
..- Also good for displaying information with markdown, such as walkthroughs
- **Spyder IDE** is useful for running longer code files; it also tracks variables (most useful for web scrapers)

## Reading in data
- Remember to import **csv** at the start
- Read in `with open`, defining and delimiting
Table used as modes for using `open`
 Character	| Meaning
:----:|:--------
`r`	| open for reading (default)
`w`	| open for writing, truncating the file first
`x`	| open for exclusive creation, failing if the file already exists
`a` |	open for writing, appending to the end of the file if it exists
`b`	| binary mode
`t`	| text mode (default)
`+`	| open a disk file for updating (reading and writing)
`U` |	universal newlines mode (deprecated)
