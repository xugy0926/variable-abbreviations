

## current 

一词多意的现象不仅在汉语中存在，在英文中也是如此，比如 current。不同语境下，current 不仅语义不同，词性也会不同。

最常见的用法是作为形容词，表达“当下、现在”的意思，语义可以近似理解为`the present time`

例如：在 [reduce（）][1]函数中出现的 `currentValue` 中， `current` 的语义就是一个形容词


```
var maxCallback = ( acc, cur ) => Math.max( acc.x, cur.x );
var maxCallback2 = ( max, cur ) => Math.max( max, cur );

// reduce() without initialValue
[ { x: 22 }, { x: 42 } ].reduce( maxCallback ); // 42
[ { x: 22 }            ].reduce( maxCallback ); // { x: 22 }
[                      ].reduce( maxCallback ); // TypeError

// map/reduce; better solution, also works for empty or larger arrays
[ { x: 22 }, { x: 42 } ].map( el => el.x )
                        .reduce( maxCallback2, -Infinity );

```
从上例中我们可以看到 current 在 JavaScript 中，往往缩写为`cur`。

---

`current` 作为名词的语义也经常会遇到，表示“流”，比如水流、电流、气流等，甚至可以用来表示民众的意见流派。

> **current**: a movement of water, air or electricity, in a particular direction:

> **current**: a particular opinion or feeling that a group of people have:



[1]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/reduce


