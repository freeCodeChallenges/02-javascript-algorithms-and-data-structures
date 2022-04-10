---
layout: home 
title: 27. Complete a Promise with resolve and reject
challengeType: 1
forumTopicId: 301196
dashedName: complete-a-promise-with-resolve-and-reject
---

<div class="row">
<div class="columnStmt" markdown="1">

## Description
------

[Home - ES6](../es6/README.md)

[Before](./26-create-a-javascript-promise.md)  | [Next](./28-handle-a-fulfilled-promise-with-then.md)

A promise has three states: `pending`, `fulfilled`, and `rejected`. The promise you created in the last challenge is forever stuck in the `pending` state because you did not add a way to complete the promise. The `resolve` and `reject` parameters given to the promise argument are used to do this. `resolve` is used when you want your promise to succeed, and `reject` is used when you want it to fail. These are methods that take an argument, as seen below.

```js
const myPromise = new Promise((resolve, reject) => {
  if(condition here) {
    resolve("Promise was fulfilled");
  } else {
    reject("Promise was rejected");
  }
});
```

The example above uses strings for the argument of these functions, but it can really be anything. Often, it might be an object, that you would use data from, to put on your website or elsewhere.

##  instructions 

Make the promise handle success and failure. If `responseFromServer` is `true`, call the `resolve` method to successfully complete the promise. Pass `resolve` a string with the value `We got the data`. If `responseFromServer` is `false`, use the `reject` method instead and pass it the string: `Data not received`.

</div>
<div class="columnSol" markdown="1">

## Solution
------

{% highlight sql linenos=table %}

{% include_relative 27-complete-a-promise-with-resolve-and-reject.js %}

{% endhighlight %}

</div>
</div>

