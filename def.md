

## default

**default**: 默认选项、缺省值，缩写为`def`

其英英释意为：

>  A particular value for a variable that is assigned automatically by an operating system and remains in effect unless canceled or overridden by the operator.

即：  缺省，默认：某一变量的特定值，由操作系统自动指定并持续有效，除非操作者取消它或使它无效。

---

来看一段来自[MDN][1]的代码：

```
function multiply(a, b) {
  return a * b;
}

multiply(5, 2); // 10
multiply(5);    // NaN !
```
遇到 b 的值为 undefined 时，会返回`NaN`

ES2015 增加的`默认参数(default parameters)`的概念可以帮我们轻松避免类似问题：
```
function multiply(a, b = 1) {
  return a * b;
}

multiply(5, 2); // 10
multiply(5);    // 5
```

[1]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Functions/Default_parameters
