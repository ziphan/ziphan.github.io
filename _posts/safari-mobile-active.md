---
title:  Safari Mobile 页面中的 :active
description: 解决 Safari Mobile 上 :active 无效的问题
---

> By default, Safari Mobile does not use the :active state unless there is a touchstart event handler on the relevant element or on the <body>

```js
document.body.addEventListener('touchstart', function (){}); //...空函数即可
```
将上述事件监听代码加上后，Safari Mobile上就可以看到按钮按下后的切换效果了。
