---
id: 587d7b7e367417b2b2512b24
title: Use the Conditional (Ternary) Operator
challengeType: 1
forumTopicId: 301181
---

# --description--

The <dfn>conditional operator</dfn>, also called the <dfn>ternary operator</dfn>, can be used as a one line if-else expression.

The syntax is:

`condition ? expression-if-true : expression-if-false;`

The following function uses an if-else statement to check a condition:

```js
function findGreater(a, b) {
  if(a > b) {
    return "a is greater";
  }
  else {
    return "b is greater";
  }
}
```

This can be re-written using the `conditional operator`:

```js
function findGreater(a, b) {
  return a > b ? "a is greater" : "b is greater";
}
```

# --instructions--

Use the `conditional operator` in the `checkEqual` function to check if two numbers are equal or not. The function should return either "Equal" or "Not Equal".

# --hints--

`checkEqual` should use the `conditional operator`

```js
assert(/.+?\s*?\?\s*?.+?\s*?:\s*?.+?/.test(code));
```

`checkEqual(1, 2)` should return "Not Equal"

```js
assert(checkEqual(1, 2) === 'Not Equal');
```

`checkEqual(1, 1)` should return "Equal"

```js
assert(checkEqual(1, 1) === 'Equal');
```

`checkEqual(1, -1)` should return "Not Equal"

```js
assert(checkEqual(1, -1) === 'Not Equal');
```

# --seed--

## --seed-contents--

```js
function checkEqual(a, b) {

}

checkEqual(1, 2);
```

# --solutions--

```js
function checkEqual(a, b) {
  return a === b ? "Equal" : "Not Equal";
}
```
