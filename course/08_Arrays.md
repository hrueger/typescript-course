# Chapter 8: Arrays
You often need to save a list of data. Using seperate variables for each value is not a very good idea, as we'd have to add new variables in the code if the list gets longer. That's why we are using arrays.

The array datatype is `Array` or `[]`. We can initialize an empty array with the two brackets `[]`, too. Like so:
```typescript
let fruits: [] = [];
```
We can also specify, which type of values will be stored in this array, for example strings:
```typescript
let fruits: string[] = [];
```
We can also populate the array with data:
```typescript
let fruits: string[] = ["apple", "banana", "coconut"];
```
Each value is seperated with a comma.

To get, update or insert values, we can use so called indices. The index of a value can be imagined as its position in the array.

Every the first element has always the index 0! It does not start with 1.

You can get a value like so:
```typescript
let fruits: string[] = ["apple", "banana", "coconut"];
console.log("My favourite Fruit: " + fruits[0]);
console.log("Another fruit I like: " + fruits[2]);
```

You can also update or insert new values:
```typescript
let fruits: string[] = ["apple", "banana", "coconut"];
console.log(fruits[0]);
fruits[0] = "New fake fruit!";
console.log(fruits[0]);
```

A very useful property of the array is its length. If you want to get the last element, you can do this:
```typescript
let fruits: string[] = ["apple", "banana", "coconut"];
console.log(fruits[fruits.length - 1]);
```
Why do you need `fruits.length - 1`? Remember, that the counting of the array indices starts at 0. So the last index is one less that its length.

## Exercise
Create a little program with a list of six colors and output the first, the third and the last color. Then, change the first color to the last color and output the first color again.

---
Now, proceed to the [next chapter](./09_For_loops.md).