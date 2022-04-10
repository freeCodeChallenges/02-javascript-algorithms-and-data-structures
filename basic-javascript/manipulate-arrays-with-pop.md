---
layout: home
title: Manipulate Arrays With pop()
challengeType: 1
videoUrl: 'https://scrimba.com/c/cRbVZAB'
forumTopicId: 18236
dashedName: manipulate-arrays-with-pop
---

<div class="row">
<div class="columnStmt" markdown="1">

## Description
------

[Basic JavaScript](../basic-javascript/README.html) 

[Before](./manipulate-arrays-with-push.md)  | [Next](./manipulate-arrays-with-shift.md) 

Another way to change the data in an array is with the `.pop()` function.

`.pop()` is used to pop a value off of the end of an array. We can store this popped off value by assigning it to a variable. In other words, `.pop()` removes the last element from an array and returns that element.

Any type of entry can be popped off of an array - numbers, strings, even nested arrays.

```js
const threeArr = [1, 4, 6];
const oneDown = threeArr.pop();
console.log(oneDown);
console.log(threeArr);
```

The first `console.log` will display the value `6`, and the second will display the value `[1, 4]`.

##  instructions 

Use the `.pop()` function to remove the last item from `myArray` and assign the popped off value to a new variable, `removedFromMyArray`.

</div>
<div class="columnSol" markdown="1">

## Solution
------

{% highlight sql linenos=table %}

{% include_relative manipulate-arrays-with-pop.js %}

{% endhighlight %}

</div>
</div>


