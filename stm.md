## Stream

**stream** 常见的用法有十来种，最常用的译法是`小溪`，`小河流`
> A stream is **a small narrow river**.

其他意思基本和“流”有关，比如，人流，车流，甚至鼻涕流
> **A stream of vehicles or people** is a long moving line of them. 

> My nose is streaming.

**注意**：stream 的缩写形式是 stm，而不是前三个字母组合 str（str 是 string 的缩写）

---

计算机里的 stream 往往指的是数据流：

计算机只认识0和1，也就是二进制数字，所有的字符串、图片、视频等信息都会首先转换为数字信息，然后转换为电脑认识的二进制格式的数据，其转换结果就是 binary data。而这些数据非常庞大的时候移动起来并不是整体一起移动，而是首先进行分割再分批移动，Node.js 中 stream 就指代的是这些二进制数据 (binary data) 的一系列有序移动。

关于 Node.js 中Buffer 和 Stream 的概念，可参考[Medium][1]，译稿[在这里][2]。

> **Stream** in Node.js simply means **a sequence of data being moved from one point to the other over time**. The whole concept is, you have a huge amount of data to process, but you don’t need to wait for all the data to be available before you start processing it.

> Basically, **this big data is broken down and sent in chunks.** So from the original definition of a buffer (“streams of binary data… in the context of… file system”) this simply means **binary data being moved** in the file system. For example, moving the texts stored in file1.txt to file2.txt.


[1]: https://medium.freecodecamp.org/do-you-want-a-better-understanding-of-buffer-in-node-js-check-this-out-2e29de2968e8
[2]: http://xugaoyang.com/post/5b915602b034ee61e48024f2

