---
title: "How to put an item at the bottom of its container using CSS"
date: 2019-08-22T07:00:00+02:00
description: "Find out how to stick an item at the bottom of its container using CSS"
tags: css
---

It's a rather common thing to do, and I had to do it recently.

I was blindly assigning `bottom: 0` to an element which I wanted to stick to the bottom of its parent.

Turns out I was forgetting 2 things: setting `position: absolute` on that element, and adding `position: relative` on the parent.

Example:

```html
<div class="container-element">
  ...
  <div class="element-to-stick-to-bottom">
    ...
  </div>
</div>
```

```css
.element-to-stick-to-bottom {
  position: absolute;
  bottom: 0;
}

.container-element {
  position: relative;
}
```
