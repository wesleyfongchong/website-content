---
title: How to remove all children from a DOM element
description: "Given a DOM element, how do you remove all its children?"
date: 2019-08-28T07:00:00+02:00
tags: browser
---

Given an item in the DOM, use [`querySelector()`](/selectors-api/) to identify it, using any CSS selector you want.

In a loop, you basically check if the `firstChild` property is defined (the element has at least a child) and you remove it.

The loop ends when all children are removed:

```js
const item = document.querySelector('#itemId')
while (item.firstChild) {
  item.removeChild(item.firstChild)
}
```