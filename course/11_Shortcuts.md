## Shortcuts
Here are some useful shortcuts for `for` loops, and for `if`, `else if` and `else` chains.

When using a `for` loop that is specifically meant to run through the contents of an array, you don't have to initialize a variable equal to the index of the array's first item, a condition that checks if the variable is equal to the index of the array's last item and incrementation of adding one to the variable. Use this short cut instead:

```typescript
let fruits: string[] = ["apple", "banana", "coconut", "dragonfruit"];
for(i in fruits){
    console.log(fruits[i]);
}
```
Isn't that a lot better? Now check this one out. When you have a really long string of `else if`s where all you're doing is repeatedly checking if a variable is equal to one thing, then another, then another, and so on, like so:

```typescript
let favoriteFruit: string = "banana";

if(favoriteFruit == "apple"){
    console.log("Favorite fruit is red");
}else if(favoriteFruit == "coconut"){
    console.log("Favorite fruit is white");
}else if(favoriteFruit == "banana"){
    console.log("Favorite fruit is yellow");
}else if(favoriteFruit == "dragonfruit"){
    console.log("Favorite fruit is pink");
}else{
    console.log("Favorite fruit is unknown");
}
```
You can shorten each case significantly using the `switch` and `case` function.

```typescript
let favoriteFruit: string = "banana";

switch(favoriteFruit){
}case("apple"){
    console.log("Favorite fruit is red");
}case("coconut"){
    console.log("Favorite fruit is white");
}case("banana")
    console.log("Favorite fruit is yellow");
}case("dragonfruit"){
    console.log("Favorite fruit is pink");
}else{
    console.log("Favorite fruit is unknown");
}
```

## Exercise
Make a program that runs through the contents of an array full of fruits, and for each fruit it outputs the color of the fruit. Done correctly, this program should use both of the shortcuts taught in this chapter.

---

Then, go on with the [next chapter](./next_chapter.md).