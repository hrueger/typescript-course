# Chapter 6: Datatypes
Have you ever wondered, why TypeScript is called TypeScript? That is because you can defined types for your variables, methods, parameters etc. This is very handy if you have a variable which must be of a specific type, for example a number, because it later gets multiplied by another number. Let's see, how it works:
```typescript
let mustBeNumeric: number = 5;
console.log("Multiplied by 10 is " + mustBeNumeric * 10)
```
You can define the type of a variable after a colon. This way, the TypeScript compiler will thow an error, if the value you want to put in the variable is the wrong type.

The following datatypes are most important and most used:

* `string`: This datatype is used for strings.
```typescript
let stringVariable: string = "Cool!";
```

* `number`: This datatype is used for number.
```typescript
let decimalValue: number = 10;
let decimalValueWithComma: number = 10.9480;
let hexaDecimalValue: number = 0xf10b;
```

* `boolean`: This datatype represents a `true` or `false` value.
```typescript
let booleanValue1: boolean = false;
let booleanValue2: boolean = true;
```

---
Now, proceed to the [next Chapter](./07_Conditions.md).