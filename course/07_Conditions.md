# Chapter 7: Conditions
Conditions are needed very often in the daily life. For example, when you have a game with ball flying in one direction and you need to check if it touches the wall.

Conditions are made with the `if` keyword followed by the condition in the parentheses. The code block, which should be run if the condition is true, is enclosed in curly braces. It can be followed by an `else if` block with another condition and / or by an `else` block.
```typescript
if (condition) {
    // do this
}
```
```typescript
if (condition) {
    // do this
} else {
    // do that
}
```
```typescript
if (condition) {
    // do this
} else if (another condition) {
    // do that
}
```
```typescript
if (condition) {
    // do this
} else if (another condition) {
    // do that
} else {
    // do another thing
}
```
You can have only one `if`, unlimited `else if` and one `else` for every if condition.

## Conditions
You can use many different conditions. The easiest ones are just comparing numbers using `<` (smaller than), `>` (greater than), `<=` (smaller or equal) and `>=` (greater or equal). Like so:
```typescript
if (myCoolNumber < 7) {
    console.log(myCoolNumber + " is smaller than seven!");
} else if (myCoolNumber < 20) {
    console.log(myCoolNumber + " is smaller than twenty!");
} else {
    console.log(myCoolNumber + " is not smaller than twenty!");
}
```

You can compare any to datatypes for equality with `==`, for example strings, numbers, booleans etc.
```typescript
if ("hi" == "hi") {
    console.log("These two strings are equal!");
}
let myVariable = false;
if (myVariable == true) {
    console.log("My Variable is true!");
} else {
    console.log("My Variable is not true!");
}
```

If you just put a variable or a value in the condition - without a operator like `==` or `>` - the value is checked for truth. That means, your condition returns true if the value is different than `undefined`, `false`, `null` or `0`.
```typescript
let myVar = undefined; // try out: undefined, null, false, true, 0 and 1
if (myVar) {
    console.log("Yes!");
} else {
    console.log("No.");
}
```
This is useful for checking if the variable has an actual value.

If you want to check if a something is not equal, or if a boolean variable is false, you can use a NOT gate. This is done simply b putting a `!` before the condition.
```typescript
if(!myCoolNumber == 7){
    //do something
}
```
```typescript
if(!condition){
    //do this
}
```
If you want to check if the variable is `false` and you don't want the condition to become true if the variable is `undefined`, `0`, or `null`, you can use the `===` operator. This one checks exactly for the following value.

## Exercise
Write a little program, that tells you if a variable is lower, greater or equal to 18.


---
Then, proceed to the [next chapter](./08_Arrays.md).