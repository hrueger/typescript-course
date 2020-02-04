# Functions
We need some way to "bundle" code we want to use multiple times. Functions can handle this job and look like this:
```typescript
function greet() {
    console.log("Hello");
}
```
It is just the word `function` followed by the name of your function. You can choose any name you want, although the same rules as for variables apply. To remember: It's only letters and underscores. This name is then followed by parentheses. The code which is inside the function is surrounded by curly brackets.

The code above is just the definition of the function. If we run the code like this, it won't do anything. We need to call our function in order to execute it. This is done like so:
```typescript
greet();
```
Now you should get the output `Hello`.

But what if we want to process the result of a function further and not directly output it? We can `return` it. Just like this:
```typescript
function addOneAndThree() {
    return 1 + 3;
}
```
If we run this function with `addOneAndThree()`, nothing happens. This is because the value is returned, but not used. To use it, we could either save it in a variable or give it to another function:
```typescript
let result = addOneAndThree();
// or
console.log(addOneAndThree());
```
We can also define the type of the returned value of our function using the `string`, `number` or other types, just like with variables:
```typescript
function addOneAndThree(): number {
    return 1 + 3;
}
```

But what if we want to give our function some values? We can do this with parameters. That looks like this:
```typescript
function greet(nameOfPerson): string {
    return "Hello " + nameOfPerson + "!"; 
}
var firstOneToGreet: string = "Peter";
console.log(greet(firstOneToGreet));
console.log(greet("Tom"));
```

We can also define the types of the parameters:
```typescript
function greet(nameOfPerson: string): string {
    return "Hello " + nameOfPerson + "!"; 
}
``` 
This way, if we try to greet a number, the TypeScript compiler will warn us.

## Exercise 1
Create a function which takes a name (string) and an age (number) as parameters and prints `name is x years old.`

## Exercise 2
Create a function which takes two numbers as parameters and prints if the product of those numbers is greater than 100 or not.

## Exercise 3
Create a function which multiplies three parameters and returns the result. Then multiply the returned value with 3 and print the result.


---

Then, go on with the [next chapter](./13_TemplateStrings.md).