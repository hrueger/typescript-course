# Chapter 9: For loops
If you want to iterate through arrays or if you want to count from one to ten, it's very bad to do it like this:
```typescript
let myFruits: string[] = ["apple", "banana", "coconut", "dragonfruit"];
console.log("Fruit with index 0: " + myFruits[0]);
console.log("Fruit with index 1: " + myFruits[1]);
console.log("Fruit with index 2: " + myFruits[2]);
console.log("Fruit with index 3: " + myFruits[3]);
```
If you add one more item to the array, you would also have to add one more console.log call. That's where loops come in handy.

The most basic loop is a for loop. It takes three inputs: initialization; condition and incrementation. The intialisation is done once before the loop starts. As we don't want to have an infinite loop, we need a condition to check whether the loop should go on or not. The increment part is run once after every round.

The loop looks kind of like a if statement, except that the three arguments are split using semicolons:
```typescript
for (initialization, condition, incrementation) {
    // your content of the loop
}
```

If we want to count from zero to nine, we would create a counter variable in the initialization part. Those counter variables are often called `i`: `let i = 0;`. If our condition returns true, the loop will go on. So we check if i is smaller than ten (because we want to count up to nine): `i < 10`. And in every round we want to increment `i` by one, so the last part is `i = i + 1`. As incrementing and decrementing by one is needed very often, you can short this to `i++` or `i--`. So our final loop looks like this:
```typescript
for (let i = 0; i < 10; i++) {
    console.log("This is round #" + i);
}
```

We can also iterate through arrays using the same technique. The only difference is, that our condition compares the counter and the length of the array. Like so:
```typescript
let myFruits: string[] = ["apple", "banana", "coconut", "dragonfruit"];
for (let i = 0; i < myFruits.length; i++) {
    console.log("This is round #" + i + " and the fruit is " + myFruits[i]);
}
```
Notice, that we check if the counter is smaller that the array's length, because the indices start with 0.

## Exercise
Create a little program, which outputs the fruits in __reversed__ order.

---

Then, go on with the [next chapter](./10_While_loops.md).