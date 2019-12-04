# Chapter 5: Variables
We always directly printed the result of our calculations and addition of strings using the methods of the console module. But what, if we want to process the result further? Or if we need it later in the program? We need to store it someware.

Variables can be imagined as little bags where we can insert things and get them back.

Variables always start with the `let` keyword followed by the varable name. A keyword is a certain word defined by the language itself, you cannot change it. You can't name your variables like the keywords, as this wouldn't make sense.

Let's create a variable and save a string in it:
```typescript
let myCoolString = "Hello!";
```
A variable name must not contain spaces or other characters like &, % etc. Only letters, numbers, underscores (`_`) and dollar signs are allowed.

If the variable name consists of multiple words, it is best practise to use camel-case-notation. That means, the first letter of every word (except the first one) is capitalized.

Now, what can we do with the variable? We can use it:
```typescript
let myCoolString = "Hello!";
console.log(myCoolString);
```
But we can also change it again:
```typescript
let myCoolString = "Hello";
console.log(myCoolString);
myCoolString = "World!";
console.log(myCoolString);
```
Notice, that the `let` keyword is missing in the third line, as the variable is already initialized. If we refer to our bag example, the bag already exists with this name, so we just put a new value into it.

## Exercise
Create a little program, which defines two variables, one with the string `"Hello World - My favourite number is "`, and the other one with the number 3. Then print everything with one `console.log()`, so that it outputs `"Hello World - My favourite number is 3"`.

---
Then, proceed to the [next chapter](./06_Datatypes.md)