![Typescript](https://www.freecodecamp.org/news/content/images/size/w2000/2020/08/1_9XMpTyccrky0eW5Wz6DoWQ.png)

> [cover image source: https://www.freecodecamp.org/news/how-to-add-typescript-to-a-javascript-project/](https://www.freecodecamp.org/news/how-to-add-typescript-to-a-javascript-project/)

Some key points to get you started with typescript, i made this as a personal note while learning typescript from [scrimba.com](scrimba.com) and i really hope it helps anyone using this.

## What is typescript

- typescript is an open-source language built on javascript, by adding static types definition to javascript.
- it is considered a superset of javascript, what this means is that it takes javascript and adds new features to it and existing valid javascript programs are also valid in typescript

## How typescript started

- typescript was developed and is maintained by microsoft

## Notes and pros of typescript

- typescript deals with types, providing essential description to the shape of an object. Providing better documentation and allows typescript validate that your code is working correctly.

- writing types in typescript is optional, typescript uses type inference to enforce types.
- typescript can be used for client and server side (backend developement, i.e with nodejs and deno)
- typescript transcompiles down to javacsript so it can run on the browser, because the browser doesn't understand typescript
- typescript has a compiler (typsecript compiler or tsc for short)
- it's more readable
- cleaner code
- makes you write code with less errors
- no need for pseudo-codes //explaining a line of code immediately before declaration

## Cons of typescript

- it requires compilation while javascript doesn't - this isn't an issue because most of javascript applications today still requires to be compiled(reactjs, etc..), there's webpack and babel that does this

## Types in Javascript

#### Primitives:

- `Boolean` : **_typeof instance === "boolean"_**
- `Number` : **_typeof instance === "number"_**
- `String` : **_typeof instance === "string"_**
- `BigInt` : **_typeof instance === "bigint"_**
- `Symbol` : **_typeof instance === "symbol"_**
- `Undefined` : **_typeof instance === "undefined"_**

#### Structural Types:

- `Object` : **_typeof instance === "object"_**
- `Function` : **_typeof instance === "function"_**

#### Structural Root Primitive:

- `null` : **_typeof instance === "object"_**

## Simple demo of using types in javascript

- using `typeOf` in javascript

```js
//targeting dom
const button = document.querySelector(".button");
const firstInput = document.querySelector("#first-input");
const secondInput = document.querySelector("#second-input");
const screen = document.querySelector(".screen");

function addNumbers(a, b) {
  if (typeof a === "number" && typeof b === "number") {
    screen.innerHTML = a + b;
  } else screen.innerHTML = parseInt(a) + parseInt(b);
}
//event listener
button.addEventListener("click", () =>
  addNumbers(firstInput.value, secondInput.value)
);
```

## Types in typescript

Typescripts supports all Javascript types and has additional types.
There are 3 commonly used types in typescript namely,

- `String` == **"hello typescript"**
- `Number` == **10**
- `Boolean` == **true or false**

Other types in typescript includes;

- `Boolean type`
- `Number type`
- `String type`
- `Object type`
- `Array type`
- `Tuple Type`
- `Enum Type`
- `Any Type`
- `Union Type`
- `Literal Type`
- `Function Type`
- `Unknown Type`
- `Never type`
- `Custom type`
