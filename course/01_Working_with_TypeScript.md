# Chapter 1: Working with TypeScript

After installing Node.js, we can use the `node package manager`, short `npm` to install all kinds of `packages`. A package is one or multiple scripts or programs, which can be used in other programs easily.

So open a command prompt and type in `npm install typescript --global`. When using the command prompt, you always type in the name of the program you want to use first, in our case `npm`. The next words are specific to the node package manager. We tell them to install the typescript package and use the flag (prefixed with --) global to tell it, that it should be not in the current project and current folder, but in a certain diretory, so that it is avalible on the whole computer.

After the installation process is completed, the `tsc` command is avalible in your command prompt. So copy the following code into a new file for example called `01_working_with_ts_01.ts` (because it's the first example or exercise in the first chapter):
```typescript
const message: string = 'Hello World!';
console.log(message);
```
Next, compile this file by typing `tsc 01_working_with_ts_01.ts` in your command prompt. It should give you a new file called `01_working_with_ts_01.js`. Notice the different file extension. This newly generated JavaScript file can now be run using the Node.js runtime environment: `node 01_working_with_ts_01.js`. It should print `Hello World!` on your screen!

## Simplifying the dev process
As we don't always want to type in `tsc filename.ts` and then `node filename.js`, there's a cool npm package called `ts-node`, which compiles and runs the TypeScript code in one single step. Let's install it globally. Do you remember, how? If not, try `npm install ts-node --global`.

Now you can run all TypeScript files just by typing `ts-node filename.ts`. Cool, right?

## Exercise
Copy the following code in a new TypeScript file with the following code and run it at least two times.
```typescript
console.log(Math.floor(Math.random()*100));
```

---
Then, proceed to the [next Chapter](./02_Printing_debug_messages.md).