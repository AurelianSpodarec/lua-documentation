## Reference
### [Global Objects](#global-objects)  
[String](#global-objects_string)  
[Math](#global-objects_math)  
[Table](#global-objects_table)  
[Coroutine](#global-objects_coroutine)  
[Operating System Facilities (OS)](#global-objects_os)  
### [Functions](#functions)  
[Independent](#functions_table)  
[Table Functions](#functions_table)  
[Files](#functions_table)  
[FIle Loaading Functions](#functions_table)  
[Error Handling Functions](#functions_table)  
### [Expressions & Operators](#expressions-and-operators)  
### [Statements & Declarations](#staatements-and-declarations)  



==========================================================================


# [Global Objects](#global-objects)  
[String](#global-objects_string)  
[Math](#global-objects_math)  
[Table](#global-objects_table)  
[Coroutine](#global-objects_coroutine)  
[Operating System Facilities (OS)](#global-objects_math)  

=======================


## <a name="global-objects_string">String</a>  
<!-- http://www.lua.org/pil/2.4.html -->
The `String` object is used to represent and manipulate a sequence of characters.

### Escape Sequences
Special characters can be encoded using escape sequences:

| Escape sequence      | Use                   |
| :---                 | :---                  |
| `\b`                 | Backspace             |
| `\f`                 | Formfeed              |
| `\n`                 | New line              |
| `\r`                 | Carriage return       |
| `\t`                 | Tab                   |
| `\v`                 | Vertical tab          |
| `\\`                 | Backslash             |
| `\"`                 | Double quotes         |
| `\'`                 | Single quotes         |
| `\[`                 | Left square bracket   |
| `\]`                 | Right square bracket  |


### Functions
[`tostring()`]
 <!-- Editor: Should this be here? -->

### Methods
[`String.byte()`](#global-objects_string-method_byte)  
[`String.char()`](#global-objects_string-method_char)  
[`String.dump()`](#global-objects_string-method_dump)  
[`String.find()`](#global-objects_string-method_find)  
[`String.format()`](#global-objects_string-method_format)  
[`String.gmatch()`](#global-objects_string-method_gmatch)  
[`String.gsub()`](#global-objects_string-method_gsub)  
[`String.len()`](#global-objects_string-method_len)  
[`String.lower()`](#global-objects_string-method_lower)  
[`String.match()`](#global-objects_string-method_match)  
[`String.pack()`](#global-objects_string-method_pack)  
[`String.packsize()`](#global-objects_string-method_packsize)  
[`String.rep()`](#global-objects_string-method_rep)  
[`String.reverse()`](#global-objects_string-method_reverse)  
[`String.sub()`](#global-objects_string-method_sub)  
[`String.unpack()`](#global-objects_string-method_unpack)  
[`String.upper()`](#global-objects_string-method_upper)  


=============


## <a name="global-objects_math">Math</a>  
<!-- https://www.lua.org/manual/5.4/manual.html#6.7 -->
Math is a built-in object that has properties and methods for mathematical constants and functions. It's not a function object.

`Math` works with `Numeric` type.

<!-- Functions with the annotation "integer/float" give integer results for integer arguments and float results for non-integer arguments. 

The rounding functions `math.ceil, math.floor, and math.modf return an integer when the result fits in the range of an integer, or a float otherwise. -->

### Static properties
[`math.pi`](#global-objects_math_static-properties_pi)  
Ratio of a circle's circumference to its diameter; approximately 3.14159. 

[`math.huge`](#global-objects_math_static-properties_huge)  
TODO: Improve - The float value HUGE_VAL, a value greater than any other numeric value.

### Methods
[`math.abs(x)`](#global-objects_math_methods_abs)  
Returns the absolute value of `x`.  

[`math.acos(x)`](#global-objects_math_methods_acos)  
Returns the arccosine of `x`.  

[`math.asin(x)`](#global-objects_math_methods_asin)  
Returns the arcsine of `x`.  

[`math.atan(x)`](#global-objects_math_methods_atan)  
Returns the arctangent of `x`.  

[`math.atan2(y, x)`](#global-objects_math_methods_atan2)  
Returns the arctangent of the quotient of its arguments.

[`math.celi(x)`](#global-objects_math_methods_celi)  
Returns the smallest integer greater than or equal 
to `x`.  
[`math.cos(x)`](#global-objects_math_methods_cos)  
Returns the cosine of `x`.  

[`math.cosh(x)`](#global-objects_math_methods_cosh)  
Returns the hyperbolic cosine of `x`.  

[`math.deg(x)`](#global-objects_math_methods_deg)  
TODO: Improve - Returns the angle `x` (given in r
adians) in degrees.  
[`math.exp(x)`](#global-objects_math_methods_exp)  
Returns `e^x`, where `x` is the argument, and e i
s Euler's constant (`2.718…`, the base of the natural logarithm).  
[`math.floor(x)`](#global-objects_math_methods_floor)  
Returns the largest integer less than or equal to `x`
.  
[`math.fmod(x, y)`](#global-objects_math_methods_fmod)  
TODO: Improve - Returns the remainder of the division 
of x by y that rounds the quotient towards zero.  
[`math.frexp(x)`](#global-objects_math_methods_frexp)  
TODO: Improve -Returns m and e such that x = m2e, e i
s an integer and the absolute value of m is in the range `[0.5, 1)` `(or zero when x is zero)`.  
[`math.ldexp(x, y)`](#global-objects_math_methods_ldexp)  
TODO: Improve - Returns m2e (e should be an integer).  

[`math.logx(x)`](#global-objects_math_methods_log)  
Returns the natural logarithm (㏒e; also, ㏑) of `
x`.  
[`math.log10(x)`](#global-objects_math_methods_log10)  
Returns the base-10 logarithm of `x`.  

[`math.max(x, ..., y)`](#global-objects_math_methods_max)  
Returns the largest of zero or more numbers.  

[`math.min(x, ..., y)`](#global-objects_math_methods_min)  
Returns the smallest of zero or more numbers.  

[`math.modf(x)`](#global-objects_math_methods_modf)  
TODO: Improve - Returns two numbers, the integral p
art of x and the fractional part of x.  
[`math.pow(x, y)`](#global-objects_math_methods_pow)  
Returns base `x` to the exponent power y (that is, `
x^y`).  
[`math.rad(x)`](#global-objects_math_methods_rad)  
TODO: Improve - Returns the angle x (given in deg
rees) in radians.  
[`math.random(x)`](#global-objects_math_methods_random)  
Returns a pseudo-random number between `0` and `1`.  

[`math.randomseed(x)`](#global-objects_math_methods_randomseed)  
TODO: Improve - Sets x as the "seed" for the pseudo-random gene
rator: equal seeds produce equal sequences of numbers.  
[`math.sinx(x)`](#global-objects_math_methods_sin)  
Returns the sine of `x`.  

[`math.sinh(x)`](#global-objects_math_methods_sinh)  
Returns the hyperbolic sine of `x`.  

[`math.sqrt(x)`](#global-objects_math_methods_sqrt)  
Returns the positive square root of `x`.  

[`math.tan(x)`](#global-objects_math_methods_tan)  
Returns the tangent of `x`.  

[`math.tanh(x)`](#global-objects_math_methods_tanh)  
Returns the hyperbolic tangent of `x`.



### Example
This section provides examples of common math operations in Lua.


=============


## <a name="global-objects_table">Table</a>
`Table` is a built in object 

### Constructor
`{}` Creates a new `Table` object.  


### Functions
[`next()`](#reference_functions_next)  
[`getmetatable()`](#reference_functions_getmetatable)  
[`setmetatable()`](#reference_functions_setmetatable)  
[`rawset()`](#reference_functions_rawset)  
[`rawget()`](#reference_functions_rawget)  
[`pairs()`](#reference_functions_pairs)  
[`ipairs()`](#reference_functions_ipairs)  

### Methods
[`Table.insert()`](#global-objects_table-method_insert)  
[`Table.remove()`](#global-objects_table-method_remove)  
[`Table.pack()`](#global-objects_table-method_pack)  
[`Table.unpack()`](#global-objects_table-method_unpack)  
[`Table.concat()`](#global-objects_table-method_concat)  
[`Table.sort()`](#global-objects_table-method_sort)  
[`Table.move()`](#global-objects_table-method_move)  

### Example
This section provides examples of common table operations in Lua.

#### Create an table


=============


## <a name="global-objects_coroutine">Coroutine</a>  
`Coroutine` is a built in object 

### Constructor
`coroutine.create()` Creates a new `Coroutine` object.

### Functions
This object does not contain specific functions.

### Methods
[`coroutine.create()`](#global-objects_coroutine-method_create)  
[`coroutine.status()`](#global-objects_coroutine-method_status)  
[`coroutine.resume()`](#global-objects_coroutine-method_resume)  
[`coroutine.running()`](#global-objects_coroutine-method_running)  
[`coroutine.wrap()`](#global-objects_coroutine-method_wrap)  
[`coroutine.yield()`](#global-objects_coroutine-method_yield)  


=============


## <a name="global-objects_os">Operating System Facilities (OS)</a>  
Description

==========================================================================










<details>
# Lua Documentation - Unofficial  🌙 
* Note: This is Work in progress

# [Lua](https://lua.org)

## What is Lua?
[Lua](https://www.lua.org/about.html) is a powerful, efficient, lightweight, embeddable scripting language. It supports procedural programming, object-oriented programming, functional programming, data-driven programming, and data description.

Lua combines simple procedural syntax with powerful data description constructs based on associative arrays and extensible semantics.
Lua is dynamically typed, runs by interpreting bytecode with a register-based virtual machine, and has automatic memory management with incremental garbage collection, making it ideal for configuration, scripting, and rapid prototyping.



## Who is Lua for?

Like with any language, choose the right tool for the job. 

Lua is rarerly used on its own, instead its usually embedded in other programs. 

Notable mentions: Roblox, Adobe Photoshop Lightroom, Angry Birds, Cheat Engine, and Garry's Mod.


Its very popular in the gaming industry but also its been used in network and system programs. 



## History of Lua

Lua was desinged by a team of of three Brazililian scientist, Roberto Ierusalimschy, Luiz Henrique de Figueiredo, and Waldemar Celes.

Brazil had a very strict import policy from 1984 untill 1992, which also included hardware. Due to the hardware limitations in Brazil, the three scientist developed the scripting language called Lua.

The first release was in 1993.

The origin of the name  and name comes from the word `luna` which is Brazilian way of saying `moon`.

Lua was slightly different and incomprated the data-description suntax of SOL, and `SOL` in Portugese means `Sun` and `Lua` meaning `Moon`.

Lua was born.


# Getting Started

Downloading Lua

# Discord Server

Join Lua Community server on discord! https://discord.gg/nNu6FeHC









==========================================================================

 <!-- Guide
Refference -->

# Lua guide
## Reference




===========================================================================

# Reference
## Built in Objects
### Tables
### Coroutine
### String
### Math
### Operating System Facilities (OS)
## Functions
### Independent
### Table Functions (like Array Methods e.g Array.map(), but just pure functions pair() used only with 'Table' aka Object )
### Files
### FIle Loaading Functions
### Error Handling Functions
## Expressions and Operators
## Statements & Declarations
 
 
 

<!-- 
<!-- 

# Table of Contents

## Variables
## Baisc Types
### Nil
### Boolean
### Number
### String
### Function
### Userdata
### Thread
### Table
## Operators
## Iterations

-- > -->


===========================================================================


# <a name="doc_statements_and_declarations">Statements & declarations<a>

## Declaration
### [variable?]
### [<const>]
## Control Flow
### [break]()
## Iterations
### [if ... then]()
### [for ... do]()
### [while .... do]()

 




## [Functions](#)
### [Select](#doc_select)
 

## [Expressions]




## [Statements]
### [local]()


### [do]()
### [else]()
### [elseif]()
### [function]()
### [end]()

### [in]()
### [repeat]()
### [then]()
### [until]()

### [true]()
### [false]()
### [return]()
### [nil]()





===========================================================================

# <a name="doc_functions">Functions</a>

## <a name="doc_functions_independent">Indepenndent</a>
`print()`  
`select()`  
`tonumber()`  
`tostring()`  
`type()`  
`collectgarbage()`  
`rawequal()`  
`rawlen()`  
## <a name="doc_table_functions">Table Functions</a>
See table functions to view the functions
## <a name="doc_functions_files">Files</a>
`load()`  
`loadfile()`  
`dofile()` 
## <a name="doc_functions_error_handling">Error Handling</a>
`assert()`  
`warn()`  
`error()`  
`pcall()`  
`xpcall()`  




===========================================================================




# <a name="doc_operators">Operators</a>

## Arithmetic Operators

Addition +
Subtraction -
Multiplication *
Division /
Modulo %
Exponentiation ^
Negation (Unary-)

Relational Operators
 

## Logical Operators

All logical operators consider `false` and `nil` nil as false, and anything else as true.

<table class="fullwidth-table">
  <caption>
    Logical operators
  </caption>
  
  <thead>
    <tr>
      <th scope="col">Operator</th>
      <th scope="col">Usage</th>
      <th scope="col">Description</th>
    </tr>
  </thead>

  <tbody>
    <tr>
      <td>
        <a href="Reference/Operators/Logical_AND"
          >Logical AND</a
        >
        (<code>and</code>)
      </td>
      <td><code>expr1 &#x26;&#x26; expr2</code></td>
      <td>
        Returns <code>expr1</code> if it can be converted to <code>false</code>;
        otherwise, returns <code>expr2</code>. Thus, when used with Boolean
        values, <code>&#x26;&#x26;</code> returns <code>true</code> if both
        operands are true; otherwise, returns <code>false</code>.
      </td>
    </tr>
    <tr>
      <td>
        <a href="Reference/Operators/Logical_OR"
          >Logical OR </a
        >(<code>or</code>)
      </td>
      <td><code>expr1 || expr2</code></td>
      <td>
        Returns <code>expr1</code> if it can be converted to <code>true</code>;
        otherwise, returns <code>expr2</code>. Thus, when used with Boolean
        values, <code>||</code> returns <code>true</code> if either operand is
        true; if both are false, returns <code>false</code>.
      </td>
    </tr>
    <tr>
      <td>
        <a href="Reference/Operators/Logical_NOT">Logical NOT </a>(<code>!</code>)
      </td>
      <td><code>not</code></td>
      <td>
        Returns <code>false</code> if its single operand that can be converted
        to <code>true</code>; otherwise, returns <code>true</code>.
      </td>
    </tr>
  </tbody>
</table>

 
## Relational Operators

Relational Operators always resolve in `true` or `false`.

<table class="standard-table">
<caption>
  Relational Operators
</caption>

<thead>
<tr>
  <th scope="col">Operator</th>
  <th scope="col">Description</th>
  <th scope="col">Examples returning true</th>
</tr>
</thead>

<tbody>
  <tr>
    <td>
      <a href="Reference/Operators#equality"
        >Equal</a
      >
      (<code>==</code>)
    </td>
    <td>Returns <code>true</code> if the operands are equal.</td>
    <td>
      <code>3 == var1</code>
      <p><code>"3" == var1</code></p>
      <code>3 == '3'</code>
    </td>
  </tr>
  <tr>
    <td>
      <a href="Reference/Operators#inequality"
        >Not equal</a
      >
      (<code>~=</code>)
    </td>
    <td>Returns <code>true</code> if the operands are not equal.</td>
    <td>
      <code>var1 != 4<br />var2 != "3"</code>
    </td>
  </tr>
    <td>
      <a
        href="Reference/Operators#greater_than_operator"
        >Greater than</a
      >
      (<code>></code>)
    </td>
    <td>
      Returns <code>true</code> if the left operand is greater than the right
      operand.
    </td>
    <td>
      <code>var2 > var1<br />"12" > 2</code>
    </td>
  </tr>
  <tr>
    <td>
      <a
        href="Reference/Operators#greater_than_or_equal_operator"
        >Greater than or equal</a
      >
      (<code>>=</code>)
    </td>
    <td>
      Returns <code>true</code> if the left operand is greater than or equal
      to the right operand.
    </td>
    <td>
      <code>var2 >= var1<br />var1 >= 3</code>
    </td>
  </tr>
  <tr>
    <td>
      <a
        href="Reference/Operators#less_than_operator"
        >Less than</a
      >
      (<code>&#x3C;</code>)
    </td>
    <td>
      Returns <code>true</code> if the left operand is less than the right
      operand.
    </td>
    <td>
      <code>var1 &#x3C; var2<br />"2" &#x3C; 12</code>
    </td>
  </tr>
  <tr>
    <td>
      <a
        href="Reference/Operators#less_than_or_equal_operator"
        >Less than or equal</a
      >
      (<code>&#x3C;=</code>)
    </td>
    <td>
      Returns <code>true</code> if the left operand is less than or equal to
      the right operand.
    </td>
    <td>
      <code>var1 &#x3C;= var2<br />var2 &#x3C;= 5</code>
    </td>
  </tr>
</tbody>
</table>





===========================================================================


# <a name="doc_string">String</a>

## Methods

`String.byte()`  
`String.char()`  
`String.dump()`  
`String.find()`  
`String.format()`  
`String.gmatch()`  
`String.gsub()`  
`String.len()`  
`String.lower()`  
`String.match()`  
`String.pack()`  
`String.packsize()`  
`String.rep()`  
`String.reverse()`  
`String.sub()`  
`String.unpack()`  
`String.upper()`  


===========================================================================


# <a name="doc_math">Math</a>

## Methods
`math.modf()`  
`math.floor()`  
`math.max()`  
`math.celi()`  



# <a name="doc_modules">Modules</a>

## Methods
`require()`
`package.config`
`package.cpath`
`package.loaded`
`package.loadlib()`
`package.path`
`package.preload`
`package.searches`


===========================================================================

# <a name="refference_functions">Functions</a>
`next()`  
`getmetatable()`  
`setmetatable()`  
`rawset()`  
`rawget()`  
`rawlen()`  
`rawequal()`  
`pairs()`  
`ipairs()`  
`assert()`  
`warn()`  
`error()`  
`pcall()`  
`xpcall()`  
`print()`  
`select()`  
`tonumber()`  
`tostring()`  
`type()`  
`load()`  
`loadfile()`  
`dofile()`  
`collectgarbage()`  






## <a name="refference_table">Tables</a>

<details>
Editor notes: Show how to loop over  the tables, how to loop over them. Instead of showing just methods, include how to use a table somewhere.
</details>

A table allows storing a collection of data under a single variable. Lua has one mechanism to represent data structure, and does not have Classes, Arrays or Objects. Every data structure is represented by tables.

Unlike in other programming languages where's the index starts from `0`, Lua starts counting from `1`. Most libraries will start with the index of `1` therefore its a good practice to follow the convetion.


### Common Usages

Tables can represent classes, arrays and objects.

#### Reasemblance of a Class, or prototyping
```lua
local Class = {}

function Class.makeSound(sound)
    return sound
end

function Class.sit()
-- code...
end

print(Class.makeSound("Woof!"))

-- Output: Woof
```

#### Reasemblance of an Array
```lua 
local array = { "Dog", "Cat", "Hippo" }
``` 

#### Reasemblance of an Object
```lua
local object = { 
    name = "John", 
    age = 25, 
    isMarried: false
}
```

```
Note: Printing a table will return table's hash such as `table: 0x5566951939f0`
```

To get a table values you need to loop over them. Check out `pairs` and `ipairs.


### Constructor 
`{}` Creates a new `table`.


### Table Functions
<!-- 
  link to functions to the functions side?
 Dont write the explanation/examples under 'table' but under 'functions'? 
-->
[`next()`](#refference_function_next)  


[`getmetatable()`](#refference_function_getmetatable)  

[`setmetatable()`](#refference_function_setmetatable)  

[`rawset()`](#refference_function_rawset)  

[`rawget()`](#refference_function_rawget)  

[`pairs()`](#refference_function_pairs)  

[`ipairs()`](#refference_function_ipairs)  


### Methods

[`table.insert()`](#object_table_insert)  
Adds one element to the table.

[`table.remove()`](#object_table_remove)  
Removes one element from the table.

[`table.pack()`](#object_table_pack)  
Packs elements into a new table.

[`table.unpack()`](#object_table_unpack)  
Unpacks a table into values.

[`table.concat()`](#object_table_concat)  
Returns a combined string from a table.

[`table.sort()`](#object_table_sort)  
Sorts the values in a table.

[`table.move()`](#object_table_move)


===========================================================================


## <a name="table-insert">Table.insert()</a>
The `table.insert()` method adds one element to the end of the table.

### Syntax
```Lua
table.insert(tbl, value)
```

### Parameter
`tbl`
The table where the item should be removed from.

`value`
The element to add to the end of the table.


### Examples

#### Adding elements to a table

```Lua

local groceries = { "Bread", "Rice" }
table.insert(groceries, "Potatoes")

-- Output:  groceries = {"Bread", "Rice", "Potatoes"}

```


**[⬆ back to top](#table-of-contents)**




# <a name="table-remove">Table.remove()</a>
The `table.remove()` method removes one element from the table and shifts it.


## Syntax
```Lua
table.remove(tbl, index)
```

## Parameter
`tbl`
The table where the item should be removed from.

`index`
The index (position) of the current element in the array.

## Examples
 Removing "Rice" from groceries table.

```Lua
groceries = { "Bread", "Rice", "Peas" }
table.remove(groceries, 2)

-- Output: groceries = { "Bread", "Peas" }
```

**[⬆ back to top](#table-of-contents)**




## <a name="table-concat">Table.concat()</a>
The `table.concat()` function is used to concatinate table values into a string.

### Syntax
```Lua
table.concat(tbl, seperator)
```

### Parameter
`tbl`
The table to be concatinated.

`seperator (optional)`
Used as a separator between values.

### Examples

#### Only table provided to the function.
```Lua
local tbl = {"The","fox","jumps","over","the","lazy","dog",}

print(table.concat(tbl)) 

-- Output: Thefoxjumpsoverthelazydog
```

```Lua
local tab = { 1, 2, 3, 4 }

print(table.concat(tab)) 

-- Output: 1234
```

#### Table provided with the second parameter

```Lua
local tbl = {"The","fox","jumps","over","the","lazy","dog",}

print(table.concat(tbl," ")) 

-- Output: The fox jumps over the lazy dog
```

```Lua
local tbl = { 1, 2, 3, 4 }

print(table.concat(tbl, "-")) 

-- Output: 1-2-3-4
```



## <a name="table-pack">Table.pack()</a>
The `table.pack()` method is used to combine values into a newly created table.

### Syntax
```
table.pack(elements)
```

### Parameters
`elements`
The values to combine into a newly created table


### Examples

This will combine all values into a new table.
```Lua
productID =  234 
productName = "Dark Chocolate"
productIngredients = { "Cocoa Mass", "Cocoa Butter", "Vanilla", "Cocoa Solids: 70% min" }

darkChocolateTable = table.pack(productID, productName, productIngredients)
 
 print(darkChocolateTable)

 -- Output: table: 0x564c9ac0a210
 ```
 
 Accessing the product igredients and getting the second one.

 ```Lua
productID =  234 
productName = "Dark Chocolate"
productIngredients = { "Cocoa Mass", "Cocoa Butter", "Vanilla", "Cocoa Solids: 70% min" }

darkChocolateTable = table.pack(productID, productName, productIngredients)
 
print(darkChocolateTable[3][2])

-- Output: Cocoa Butter
 ```

**[⬆ back to top](#table-of-contents)**





## <a name="table-unpack">Table.unpack()</a>

The `table.unpack()` returns all values from a table.

### Syntax

```Lua
table.unpack(tbl)
```

### Parameters
`tbl`
The table to be unpacked.

### Examples

Unpacking a table
```Lua
groceries = { "Bread", "Rice", "Peas" }
print(table.unpack(groceries))

-- Output: Bread Rice Peas
```

Unpacking a table with tables inside
```Lua
groceries = {
    {
        id = 31,
        name = "Bread",
        quantity = 2
    },
    {
        id = 242,
        name = "Rice",
        quantity = 1
    },
    {
        id = 493,
        name = "Peas",
        quantity = 1
    }
}

print(table.unpack(groceries))

-- Output: table: 0x55db576a62a0 table: 0x55db576a4dd0 table: 0x55db941a4dd1
```

**[⬆ back to top](#table-of-contents)**





## <a name="table-sort">Table.sort()</a>

The `table.sort()` sorts a table and returns its value sorted. If no value is provited, the sort function will default to alphabetical sorting.


### Syntax
```Lua
table.sort(tbl)

table.sort(tbl, value)
```

### Parameters



### Examples



**[⬆ back to top](#table-of-contents)**



----------------------------------

# Comments

## Single line comments

```Lua
-- 
```

## Multi-line comments

```Lua
--[[
    


--]]
```


# Semicolons
Lua doesn't require semicolons, but you're free to put them if you want.


----------------------------------

# Plugins

## Table 
table.clear()


## JSON
link to JSON decoder - http://dkolf.de/src/dkjson-Lua.fsl/home























































































----------------------------------


# I'm looking for a
## Class
## Array


<details>


<summary>.</summary>


# Template


# Name
Description what it does

## Syntax
## Parameters
## Examples


notes
.
.
.
.
.
.
.












@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@


# Lua Guidelines
It seems like general Lua programmers code seems to follow PHP style


## Variables
## Operators and comparison
## 



------------------------------------

# Variables

groceries
groceries <const>



Moon theme, because Lua is Luna/Moon

https://www.tutorialspoint.com/execute_Lua_online.php
https://www.typingclub.com/

https://developer.mozilla.org/en-US/docs/MDN/Guidelines/Code_guidelines/JavaScript

@@@@

Lua com

21 reserved words
1 mechanism to represent data struture

Lua is a dynamic language, not type anotations needed


https://Luarocks.org/


If you're comning from a language such as JavaScript or PHP, some differences are worth noting
```
Count starts from 1 not 0
0 does not mean false
1 does not mean true
```

@@@@


coroutine.create() - suspend and resume code
coroutine.yeld() - puse
courutine.resume() - continue executoin

# Reserved words



# Other
## const
 
## pairs
## ipairs
## next
## rawset
## count















<!-- Docs to look at: React, Laravel, JS MDN -->

Use real life examples, not some foo bar, a, e, i... 

 

 
<const>

# Variables

In Lua to declaare a variable you simply write out the name

`variable`

if you want to you can also

`variable <const>`

# Scope

# Functions

# Tables aka Objects & Arrays

Lua doesn't have objects nor arrays - it has just tables. s
Tables in Luas is Arr
Objects in Lua are called Tables. 
Objects in Lua are called Arrays.They serve as an array and object.

To insert into the database, you need to `table.insert(table, value)`

To unpack values from a table, you need to unpack(data)

If you print a table, you will see table hash therefore you need to use special pairs and ipairs to show the content


<!-- object.getHash() -->
<!-- object.print() -->
<!-- object.count() -->
<!-- object.insertTo(object, data) -->
<!-- object.removeFrom(data, index) -->
<!-- object.unpack(data) -->
<!-- object.returnHashes() -->
<!-- object.create -->

<!-- Lua utility -->

To access properties of tables, you need to use special functions. pairs and ipairs.

Here are a few ways to work with them.

JavaScript Example
```js


```

Lua Example
```

```


LUA Example
```
local people = {
    test = {
    ['99'] = {
         name = "Fred",
         address = "16 Long Street",
         phone = "123456"
     },
     ['8989'] = {
         name = "Wilma",
         address = "16 Long Street",
         phone = "123456"
        }
    }
}
```
  
--   for index, data in pairs(people.test) do
--       print(index)
  
--       -- for key, value in pairs(data) do
--       --     print('\t', key, value)
--       -- end
--   end
  
  -- hash breaks this 





lunavel.com

Lunavel, the unofficial documentation you were looking for Luna!
Get started


Asigning Values

Reading values

Good/Bad pratcie

Creating your own functions 







Built-In Globals
Lua Globals
Roblox Globals

Lua Libraries
coroutine
debug
math
os
string
table
utf8
bit32


# Working with JSON



# Have plugins
Copy and paste it in your file app/illuminate

- JSON - ability to decode JSON into Lua
- Table [ print table Content], not just hash









# Getting Started

## Meet Lua
Lua is a scripting language ...


### Why Lua?

What is Luna

#### Flexibile

### Starter Kits
<!-- Table addons plugin -->
<!-- JSON plugin -->


# Data Types
nil
boolean
number
string
function
userdata
thread
table

# Declearing Variables

groceries = {}
groceries <const> = {}


https://stackoverflow.com/questions/4880368/how-to-delete-all-elements-in-a-Lua-table
# Statements and declerations





## Classes

## JSON
<!-- Lua doens't provide support for JSON, however there' is a package you can install to get support for it -->

<!-- Accessing values in tables -->


# Method explore - example
Short info 

<!-- list all methods  -->


# Property definition - Example Framework 
Explanation about the feature
<!-- Demo -->

## Syntax
<!-- code -->

## Description


## Examples







<!-- http://Lua-users.org/wiki/TablesTutorial -->
<!-- https://developer.roblox.com/en-us/articles/Metatables -->
<!-- https://www.Lua.org/pil/19.2.html -->


</details>

</details>