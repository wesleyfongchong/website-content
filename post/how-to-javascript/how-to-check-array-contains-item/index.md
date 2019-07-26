---
title: How to check if a JavaScript array contains a specific value
description: "Given a JavaScript array, how do you check if it contains a specific item?"
date: 2019-08-29T07:00:00+02:00
tags: js
---

Use the `includes()` method on the array instance.

For example:

```js
['red', 'green'].includes('red') //true ✅

['red', 'green'].includes('yellow') //false ❌
```