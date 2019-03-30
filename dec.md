

## decrease

decrease 的语义是：减少；缩写：dec。反义词是 increase (inc)。

---

另外一组词我们也经常见到：**increasement/decreasement** 自增/自减。 

代码示例（来自犀牛书）：

```
//JavaScript defines some shorthand arithmetic operators

var count = 0; // Define a variable
count++; // Increment the variable
count--; // Decrement the variable
```

---
词性的角度来讲，increase/decrease 都既可以作为名词也可以作为动词使用；increment/decrement 也是，虽然以"ment"结尾，但也可以充当动词词性使用，比如MDN上对 decrement 的解释：

> #### Decrement (--)
The decrement operator decrements (subtracts one from) its operand and returns a value.
>- If used postfix (for example, x--), then it returns the value before decrementing.
> - If used prefix (for example, --x), then it returns the value after decrementing.

---

另外，[Ramda][1] 中也专门用inc和dec表示来定义自增、自减的函数。

- R.inc(42); //=> 43
- R.dec(42); //=> 41

[1]: https://ramdajs.com/docs/#dec
