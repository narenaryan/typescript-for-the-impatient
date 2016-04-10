# Types 

We all know that Java Script has only one type called <b>var</b>. All other variables which are not declared as <b>var</b> are of global scope. One more interesting thing is JavaScript has function scope whereas other traditional languages has block scope. Now we are going to see the rich set of types available in Type Script. There are three main types in TypeScript.

### <span style="color:#0086b3;">Basic Types</span>

* number
* string
* boolean

All the values which TypeScript process will fall under one of these three types. Let us see few examples of these.

```             
var name: string = "Naren Arya";
var age: number = 24;
var score: number = 8.3;
var isMarried: boolean = false;

```
If we see the above statements a variable declaration in TypeScript is happening using types attached after the variable declaration.

So if we try to store a string in integer type variable, TypeScript throws an error warning saying that we cannot store string in a number;

```
age = "Twenty-Three";

error: cannot store string type in number
```

### <span style="color:#0086b3;">More Types</span>
By extending these basic types we can have more advanced types like arrays, tuples, enums in the TypeScript.

```
var myNumberArray: number[] = [1,2,3,4,5];
var myStringArray: string[] = ["one","two","three"];
```
If we try to assign a different value to the particular type we will see an error.

```
myStringArray[2] = 5;
error: Cannot store number type in string
```

But, how we can relax this typing whenever required. Here comes the <b>any</b> key word.

### <span style="color:#0086b3;">'any' type</span>
<b>any</b> keyword is used to declare a variable which can hold any type. Normally we see such thing in dynamic programming languages. A variable can hold many types in it.
```
var noIdea: any = 22;
noIdea = false; // can hold boolean type
noIdea = "Second Guess"; // can even hold string type
```
### <span style="color:#0086b3;">The classic enumerate type</span>
<b>enum</b> type is available in the Type Script to use informative names instead of magic numbers in our code.
```
// Declaring Enumerate in type script
enum direction = {EAST, WEST, NORTH, SOUTH};

// Here EAST will have a value 0
var east_direction = direaction.EAST;

// We can also get direction from value
var south_direction = direction[4];
```

