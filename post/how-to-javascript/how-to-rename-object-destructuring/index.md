---
title: "How to rename fields when using object destructuring"
date: 2019-08-24T07:00:00+02:00
description: "Find out how to rename an object field while destructuring"
tags: js
---

Sometimes an object contains some set of properties, but you want to [destructure](/javascript-destructuring/) it changing the names.

For example some function name does not suit your naming convention, or you already have a variable with that name.

You can rename one of the fields using this syntax:

```js
const person = {
  firstName: 'Tom',
  lastName: 'Cruise'
}

const { firstName: name, lastName } = person

name //Tom
lastName //Cruise
```