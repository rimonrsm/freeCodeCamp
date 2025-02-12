---
id: 56533eb9ac21ba0edf2244c3
title: Присвоєння з поверненим значенням
challengeType: 1
videoUrl: 'https://scrimba.com/c/ce2pEtB'
forumTopicId: 16658
dashedName: assignment-with-a-returned-value
---

# --description--

Якщо пригадати з нашої розмови про <a href="/ukrainian/learn/javascript-algorithms-and-data-structures/basic-javascript/storing-values-with-the-assignment-operator" target="_blank" rel="noopener noreferrer nofollow">збереження значень за допомогою оператора присвоєння</a>, все, що знаходиться праворуч від знака рівності вирішено ще до того, як значення буде присвоєне. Це означає, що ми можемо взяти повернене значення функції та присвоїти його змінній.

Assume we have defined a function `sum` which adds two numbers together.

```js
ourSum = sum(5, 12);
```

Calling the `sum` function with the arguments of `5` and `12` produces a return value of `17`. This return value is assigned to the `ourSum` variable.

# --instructions--

Викличте функцію `processArg` з аргументом `7` та присвойте її повернене значення до змінної `processed`.

# --hints--

`processed` повинна мати значення `2`

```js
assert(processed === 2);
```

Ви повинні присвоїти `processArg` до `processed`

```js
assert(/processed\s*=\s*processArg\(\s*7\s*\)/.test(code));
```

# --seed--

## --after-user-code--

```js
(function(){return "processed = " + processed})();
```

## --seed-contents--

```js
// Setup
let processed = 0;

function processArg(num) {
  return (num + 3) / 5;
}

// Only change code below this line

```

# --solutions--

```js
var processed = 0;

function processArg(num) {
  return (num + 3) / 5;
}

processed = processArg(7);
```
