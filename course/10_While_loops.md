# While loops
A slightly simpler version of a loop, is a `while()` loop. A while loop is given a condition between the parenthesis, and runs continuosly until the condition is met. The most common use of this is when you want to run something over and over until you get a certain result, like asking for a passcode.

```typescript
let access: boolean = false;
let code: number;
while (!access) {
    code = // ask user for passcode
    if (code == 19380724) {
        access = true;
    }
}
// where access determines whether the passcode has been entered correctly, and 19380724 is the correct passcode
```

In this example, the `while()` loop will check whether access is true or false, see that it is false, and therefore run the loop's contents. After running, it will once again check to see if it's condition is still met, and if it is (if `access` is still false) it will run again, and again and again until the user gets the passcode right. There is nothing tracking how many times the loop runs.

If you just type in `while(true)` and leave the condition like that, the loop will run infinitely, because `true` is always true. This is actually very useful, especially since you can still end the loop in other ways: for example, the `break` command. Before we explain that, it's worth noting that if you type in `while(false)`, the loop simply won't run even once, because `false` always is false. Now, on to the `break` command.

If you want to stop running a while loop in the middle of it, instead of running to the end of the loop, checking the condition, and only then realizing that it is no longer met, you can use the `break` command. It instantly stops running the loop and moves on to whatever code is after, without finishing the current iteration of the loop.

```typescript
let code: number;
while (true) {
    code = // ask user for passcode
    if (code == 19380274) {
        break;
    }
    console.log("Incorrect. Try again.");
}
console.log("Correct. Access granted.")
```

Another useful tool is the `continue` command. It is similar to the `break` command in that it instantly skips the entire rest of the current iteration of the loop, but after that, instead of ending the loop, it starts it again.

```typescript
let fruits: string[] = ["apple","coconut","apple","banana","coconut","dragonfruit"]
let count: number = 0;

for (n = 0; n <= fruits.length - 1; n++) {
   if (fruits[n] == "apple") {
      continue;
   }
   count++;
}
console.log (" The number of fruits that are not apples is: " + count)
```

## Exercise
Make a loop that picks a random number from 1 to 100, and have it run continuously until it lands on 42.

---

Then, go on with the [next chapter](./11_Shortcutss.md).