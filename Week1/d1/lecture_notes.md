# Lecture Notes 1

### Ruby Environment

To see if you have ruby downloaded correctly, type in your console: `#ruby -v`. The output should be the version of Ruby you are running, for example <b> ruby 2.0.0p648 </b>

There are a couple of ways to run your ruby program: 
- You may save your code in a .rb file, then type `ruby filename.rb` terminal to execute your code. This is similar to Javascript's `node filename.js`.
- To run ruby from terminal, type `irb`, which stands for <b>Interactive Ruby</b>. This is a REPL to read and execute Ruby code from the terminal, much like node in Javascript. To exit irb, type `exit`.

Example:
```
> irb
> puts 1 + 2
3 
```

### Ruby Data Types
- Numbers: integer and float
- Strings
- Booleans
- Symbols
- Arrays
- Hashes

#### Numbers

Unlike is JavaScript, numbers in Ruby are separated into <b>integers</b> and <b>floats</b>.

- Integers are whole numbers, and return whole numbers when manipulated with mathematical operators. 
```
> puts 1 + 2
3
> puts 9 / 3
3
> puts 10 / 3
3
```

- Floats contain decimals and likewise return floats. If there is both an integer and a float in an expression, the result will be a float.
```
 > puts 1.0 + 2
 3.0
 > puts 9 / 3.0
 3.0
 > puts 10.0 / 3.0
 3.3333333...
```

#### Strings

Strings represent text and are enclosed with `" "` or `' '` interchangeably. Like is JS, strings can be concatenated using `+` but unlike in JS, you can multiply strings with a number:
```
> "Hello " * 3
"Hello Hello Hello"
```

There is no NaN in ruby; if you try to add a number to a string, ruby does not convert the number to a string, instead, a TypeError occurs.

### Variables

Declare variables by assigning them: `myVar = 1` or `hello_string = "Hello" `. You can also have the user input a variable by using `gets` or `gets.chomp`. `.chomp` removes the newline from the input.

### Useful Methods

#### Input/Output
- `puts`, `gets`, `.chomp`,
- var.to_i, to_f, to_s

#### Math
- +, -, *, /, %

#### Comparison
- >, <, >=, <=, ===, !==

#### Strings
- `.upcase`
- `.downcase`
- `.capitalize`
- `.length`
- `.index( #insert string here )`
- `+`

### Creating a Function

General Syntax:

```
def function_name arg1, arg2, ... , argN
 { code }
 end
```

Calling the function:
```
> function_name arg1, arg2 ... argN
output
```

