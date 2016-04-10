##Functions
FUnctions are the key elements in any programming language. In JavaScript we know that functions allow us to do virtually anything. Even the classic prototype object should be used in JS with functions to implement OOP. Type-Script showed very much care in designing many variations of functions that improves readability and type-safe.

In plain JavaScript we can write function definition as simple as this.

```
function add(arg1, arg2, arg3){
return arg1 + arg2 + arg3;
}
```
The main drawback of this function is it can take any type of arguments. So if we design this function only for integers, it can also serve for strings as well.

```
add(1,2,3); // returns 6
add("Naren", "Arya"); // returns NarenAryaundefined
```
At that time we should explicitly handle that case by checking type of each argument.Type Script provide a better syntactical type check at compile time to verify only arguments of allowed types are passed or not.

```
function add(arg1: number, arg2: number, arg3: number) : number {
return arg1 + arg2 + arg3;
}

add(1,2,3); // works
add(1,2,"Naren") // Error: supplied signature doesn't match
```


