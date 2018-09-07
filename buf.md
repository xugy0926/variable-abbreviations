
## Buffer 

做计划的时候，原本1个小时的工作量，很多人会预留出70分钟，多出来的10分钟就可以当做是 buffer；做预算也是如此，计划消费1000元，但是会准备1200元，这多出来的200也可以称作是buffer。

计算机术语中关于 buffer 的解释如下：
> A **buffer** is an area in a computer's memory where information can be stored for a short time. 

关于 Node.js 中Buffer 和 Stream 的概念，可参考[Medium][1]，译稿[在这里][2]。

下面节选的英文部分真的解释得很清晰，很形象，多一丢丢耐心，你一定会有所收获。

> We’ve seen that **a stream of data** is the movement of data from one point to the other, but how exactly are they moved?

> Typically, the movement of data is usually with the intention to process it, or read it, and make decisions based on it. But there is a minimum and a maximum amount of data a process could take over time. So if the rate the data arrives is faster than the rate the process consumes the data, the excess data need to wait somewhere for its turn to be processed.

> On the other hand, if the process is consuming the data faster than it arrives, the few data that arrive earlier need to wait for a certain amount of data to arrive before being sent out for processing.

> **That “waiting area” is the buffer!** It is a small physical location in your computer, usually **in the RAM,** where data are temporally gathered, wait, and are eventually sent out for processing during streaming.

> **We can think of the whole stream and buffer process as a bus station.** In some bus stations, a bus is not allowed to depart until a certain amount of passengers arrive or until a specific departure time. Also, the passengers may arrive at different times with different speed. Neither the passengers nor the bus station has control over passengers’ arrival at the station.

> In any case, passengers who arrive earlier will need to wait until the bus station decides to send the bus on its way. While passengers who arrive when the bus is already loading or when the bus has already departed need to wait for the next bus.

> In whatever the case may be, **there is always a waiting place. That is the Buffer to Node.js!** Node.js can’t control the speed or time of data arrival, the speed of the stream. It only can decide when it’s time to send out the data. If it’s not yet time, Node.js will put them in the buffer — **the “waiting area”** — a small location in the RAM, until it’s time to send them out for processing.

> A typical example where you could see buffer in action is when you’re streaming a video online. If your internet connection is fast enough, the speed of the stream will be fast enough to instantly fill up the buffer and send it out for processing, then fill another one, and send it out, then another, and yet another… till the stream is finished.

> But if your connection is slow, after processing the first set of data that arrived, the video player will display a loading icon, or display the text “buffering”, which means gathering more data, or waiting for more data to arrive. And when the buffer is filled up and processed, the player shows the data, the video. While playing that, more data will continue to arrive and wait in the buffer.

> If the player is done processing or playing the previous data, and the buffer is not yet filled up, the text **“buffering”** will be displayed again, waiting to gather more data to process.

> That is Buffer!

> From the original definition of a buffer, it shows that while in the buffer, we can manipulate or interact with the binary data being streamed. What kind of interaction could we possibly have with this raw binary data? The Buffer implementation in Node.js provides us with a whole list of what is doable. Let’s see some of them.


下面示例代码中就是在用 `buf` 来充当 buffer 的缩写。
```
// Create an empty buffer of size 10. 
// A buffer that only can accommodate 10 bytes.
const buf1 = Buffer.alloc(10);
// Create a buffer with content
const buf2 = Buffer.from("hello buffer");
```

对 Node.js 的Buffer 感兴趣的同学，可以继续戳[官网][3]了解更多。

[1]: https://medium.freecodecamp.org/do-you-want-a-better-understanding-of-buffer-in-node-js-check-this-out-2e29de2968e8
[2]: http://xugaoyang.com/post/5b915602b034ee61e48024f2
[3]: https://nodejs.org/dist/latest-v8.x/docs/api/buffer.html





