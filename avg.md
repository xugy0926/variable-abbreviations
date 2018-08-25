


当你看到代码里出现 `arr` 的时候，潜意识地认为它就是 `array`，当你看到 `avg` 的时候呢？比如下面的代码：

```
Array.prototype.avg = Array.prototype.avg || function () {
  return this.sum()/this.length; 
};
```

再比如：

```
var sum, avg = 0;

// dividing by 0 will return Infinity
// arr must contain at least 1 element to use reduce
if (arr.length)
{
    sum = arr.reduce(function(a, b) { return a + b; });
    avg = sum / arr.length;
}

document.write("The sum is: " + sum + ". The average is: " + avg + "<br/>");
```

下次看到`avg`的时候也应该条件反射式地理解为 `average/平均值`喔


顺便，来记一波数学/统计常见的英文词汇吧：

> 
 - add: 加
 - substract: 减
 - multiply: 乘
 - divide：除
 - sum: 求和
 - mean: 均值
 - median：中值
 - odd: 奇数
 - even: 偶数
 - square: 平方
 - square root: 平方根
 - decimal: 小数
 - decimal point: 小数点
 - denominator: 分母
 - numerator: 分子
 - positive: 正
 - negative: 负
 - factorial: 阶乘
 - logarithm: 对数
 - exponent: 指数、幂
 
 

