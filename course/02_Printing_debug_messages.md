# Chapter 2: Printing debug messages
As our compiled TypeScript code runs inside the Node.js runtime and not in a browser, we can't modify parts of a website. So we need another way of showing information, that we can see, if our program works.
This is done using the `console` module, which is built in, so we don't need to install anything.
This module provides multiple methods, but we're going to use the following four:
```typescript
console.log("A cool log message");
console.info("A informative info message");
console.warn("A semi-cool warning message");
console.error("A maybe unwanted error message");
```
Fortunately, the method names clearly tell us, what they are used for.

It is best practise, to end every line in TypeScript with a semicolon, but you can also leave it out if you want to.

## Exercise
Create a little program, that outputs one warning and two info messages!

# Comments
Sometimes you want to write comments in the code. Those can be for documentation or information purposes. You prefix one-line-comments with two slashes `//`. Multiline comments are put between `/*` and `*/`. The TypeScript compiler will ignore them.
```typescript
console.log("The following comment will be ignored!");
// This is a single line comment
/* This
comment
takes
multiple
lines */
console.log("Did you see any output of these comments?");
```

---
Now, proceed to the [next chapter](./03_Strings.md).