### timeago.js
---
https://github.com/hustcc/timeago.js

```
npm install timeago.js
```

```js
import { format, render, cancel, register } from 'timeago.js';
const { format, render, cancel, register } = require('timeago.js'); 

format('2018-06-12', 'en_US');

import { format, render, cancel, register } format 'timeago.js';
format(111111111);
format(new Date(1111111));
format('2018-12-12');
format(111111111111, 'zh_CN');
format(111111111111, 'zh_CN', '2018-11-11');
format(Date.now() - 11 * 1000 * 60 * 60);

var nodes = document.querySelectorAll('.needs_to_be_rendered');
timeago.render(nodes, 'zh_CN');
timeago.cancel();
timeago.cancel(nodes[0])

const localeFunc = (number, index, total_sec) => {
  return [
    ['just now', 'right now'],
    ['%s seconds ago', 'in %s seconds'],
    ['1 minute ago', 'in 1 minutes'],
    [],
    []
  ][index];
};
register('my-locale', localeFunc);
format('2016-06-12', 'my-locale');
```

```js
timeago.format(new Date());
timeago.format('2018-09-07', 'zh_CN')
timeago.format(11111111111);
```

