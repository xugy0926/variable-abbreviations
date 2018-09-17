
## column

column 的简写很好记，前三个字母： `col`。

---
熟悉 HTML 的小伙伴对 `<col>` 一定不会陌生, [MDN][1] 给出这样的说明：
> The HTML `<col>` element defines a column within a table and is used for defining common semantics on all common cells. It is generally found within a <colgroup> element.

比如：
```
    <colgroup>
        <col>
        <col span="2" class="batman">
        <col span="2" class="flash">
    </colgroup>
```
---
同样的，[Bootstrap][2] 中也会经常见到`col`和`col-`：

比如：
```
    <div class="col">
      1 of 3
    </div>
    <div class="col-6">
      2 of 3 (wider)
    </div>
    <div class="col">
      3 of 3
    </div>
```
---

其实`column`本身是建筑中`柱子`的意思:

> A **column** is a tall, often decorated cylinder of stone which is built to honour someone or forms part of a building. 

引申为跟`柱状体`相关的都可以用`a column of`表达：
> A **column** is something that has a tall narrow shape. 

甚至 
> a **column** of refugees


还有一个很常见的意思是报纸杂志的`专栏`，`专栏作家`就是`columnist`

> In a newspaper or magazine, a **column** is a section that is always written by the same person or is always about the same topic. 

---
【微软计算机词典】对`column`给出了两种解释：

第一种情况用于描述电子表格的纵列（用来描述横列的是`row`）
> A series of items arranged vertically within some type of framework—for example, a continuous series of cells running from top to bottom in a spreadsheet, a set of lines of specified width on a printed page, a vertical line of pixels on a video screen, or a set of values aligned vertically in a table or matrix.

第二种情况用于关系数据库的属性名

> In a **relational database** management system, the name for an attribute. The collection of column values that form the description of a particular entity is called a tuple or row. A column is equivalent to a field in a record in a nonrelational file system.

[1]: https://developer.mozilla.org/en-US/docs/Web/HTML/Element/col
[2]: https://getbootstrap.com/docs/4.0/layout/grid/
