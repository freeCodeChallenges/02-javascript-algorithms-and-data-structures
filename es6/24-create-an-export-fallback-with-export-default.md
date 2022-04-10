---
layout: home 
title: 24. Create an Export Fallback with export default
challengeType: 1
forumTopicId: 301199
dashedName: create-an-export-fallback-with-export-default
---

<div class="row">
<div class="columnStmt" markdown="1">

## Description
------

[Home - ES6](../es6/README.md)

[Before](./23-use--to-import-everything-from-a-file.md)  | [Next](./25-import-a-default-export.md)

In the `export` lesson, you learned about the syntax referred to as a <dfn>named export</dfn>. This allowed you to make multiple functions and variables available for use in other files.

There is another `export` syntax you need to know, known as <dfn>export default</dfn>. Usually you will use this syntax if only one value is being exported from a file. It is also used to create a fallback value for a file or module.

Below are examples using `export default`:

```js
export default function add(x, y) {
  return x + y;
}

export default function(x, y) {
  return x + y;
}
```

The first is a named function, and the second is an anonymous function.

Since `export default` is used to declare a fallback value for a module or file, you can only have one value be a default export in each module or file. Additionally, you cannot use `export default` with `var`, `let`, or `const`

##  instructions 

The following function should be the fallback value for the module. Please add the necessary code to do so.

</div>
<div class="columnSol" markdown="1">

## Solution
------

{% highlight sql linenos=table %}

{% include_relative 24-create-an-export-fallback-with-export-default.js %}

{% endhighlight %}

</div>
</div>

