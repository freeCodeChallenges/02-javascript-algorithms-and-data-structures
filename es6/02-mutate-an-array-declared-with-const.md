---
layout: home 
title: 02. Mutate an Array Declared with const
challengeType: 1
forumTopicId: 301206
dashedName: mutate-an-array-declared-with-const
---

<div class="row">
<div class="columnStmt" markdown="1">

## Description
------

[Home - ES6](../es6/README.md)

[Before](./01-compare-scopes-of-the-var-and-let-keywords.md)  | [Next](./03-prevent-object-mutation.md)

If you are unfamiliar with `const`, check out [this challenge](/learn/javascript-algorithms-and-data-structures/basic-javascript/declare-a-read-only-variable-with-the-const-keyword).

The `const` declaration has many use cases in modern JavaScript.

Some developers prefer to assign all their variables using `const` by default, unless they know they will need to reassign the value. Only in that case, they use `let`.

However, it is important to understand that objects (including arrays and functions) assigned to a variable using `const` are still mutable. Using the `const` declaration only prevents reassignment of the variable identifier.

```js
const s = [5, 6, 7];
s = [1, 2, 3];
s[2] = 45;
console.log(s);
```

`s = [1, 2, 3]` will result in an error. The `console.log` will display the value `[5, 6, 45]`.

As you can see, you can mutate the object `[5, 6, 7]` itself and the variable `s` will still point to the altered array `[5, 6, 45]`. Like all arrays, the array elements in `s` are mutable, but because `const` was used, you cannot use the variable identifier `s` to point to a different array using the assignment operator.

##  instructions 

An array is declared as `const s = [5, 7, 2]`. Change the array to `[2, 5, 7]` using various element assignments.

</div>
<div class="columnSol" markdown="1">

## Solution
------

{% highlight sql linenos=table %}

{% include_relative 02-mutate-an-array-declared-with-const.js %}

{% endhighlight %}

</div>
</div>

