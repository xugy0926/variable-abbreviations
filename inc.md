
## increase

increase 的语义是：增加；缩写：`inc`。反义词是 decrease (`dec`)

既可以当动词用，也可以充当名词词性，需要注意的是`increase`后面的介词不同，语义也会有很大差异。

- increase to: “增加到...”。比如，体重增加到60kg: incease to 60kg
- increase by: “增加了...”。比如，工资涨了500块: increase by $500
- increase in: "...的增加"。比如，涨工资: increase in salary （此时 increase 是名词词性）

---

另外一组词我们也经常见到：`increasement/decreasement`。
维基百科对`increament`的解释如下，它和`increase`相似但不完全一致：

> An increment is an increase, either **of some fixed amount**, for example **added regularly**, or of a variable amount

代码示例（来自犀牛书）：
```
//JavaScript defines some shorthand arithmetic operators

var count = 0; // Define a variable
count++; // Increment the variable
count--; // Decrement the variable
```
---

另外，[Ramda][1] 中也专门用`inc`和`dec`表示来定义自增、自减的函数。

```
R.inc(42); //=> 43
R.dec(42); //=> 41
```

[1]:https://ramdajs.com/docs/#inc
