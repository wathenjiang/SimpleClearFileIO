# 文件 I/O 简明概述

文件 I/O 性能是后台应用的主要瓶颈之一，一直以来想对文件 I/O 这个偌大的系统进行总结，故写此文。

文件 I/O 内容较多，书籍的意义在于能更系统地说明问题，避免博客文章散乱的问题。

书籍有涉及很大部分非原创内容，相关引用会在 REFERENCE 小节中指出。

书籍内容包括：

- [1.page cache](1. page cache.html)
- [2.DMA 与零拷贝技术](2. DMA 与零拷贝技术.html)
- [3.mmap](3. mmap.html)
- [4.文件分区](4. 文件分区.html)
- [5.Java ByteBuffer与 Channel](5. Java ByteBuffer与 Channel.html)
- [6.FileChannel](6. FileChannel.html)
- [7.JavaVisual 工具](7. Visual VM.html)
- [8.Java ByteBuffer 测试](8. Java ByteBuffer 测试.html)
- [9.如何实现顺序读写](9. 如何实现顺序读写.html)

一些章节可能会需要一定的 Java 语言基础，其中：1~4 小节完全不需要 Java 基础，而 5~9 小节会涉及一定的 Java 代码。读者朋友可以有选择性地阅读。



![linux_io_stack_diagram](images/linux_io_stack_diagram.jpg)

> Figure1.Linux IO Stack Diagram

---

**其他**

- 个人博客地址：[https://spongecaptain.cool](https://spongecaptain.cool/)

- 书籍 GitHub 地址：[https://github.com/Spongecaptain/SimpleClearFileIO](https://github.com/Spongecaptain/SimpleClearFileIO)，如有意见或者建议，特别希望读者朋友能够提 issue&pr。若有帮助，欢迎 star&fork。

**推荐阅读**

1. [On Disk IO, Part 1: Flavors of IO](https://medium.com/databasss/on-disk-io-part-1-flavours-of-io-8e1ace1de017)
2. [On Disk IO, Part 2: More Flavours of IO](https://medium.com/databasss/on-disk-io-part-2-more-flavours-of-io-c945db3edb13?)
3. [Read, write & space amplification - pick 2](http://smalldatum.blogspot.com/2015/11/read-write-space-amplification-pick-2_23.html)

**致谢**

本书受到 [文件 IO 操作的一些最佳实践](https://www.cnkirito.moe/file-io-best-practise/) 一文启发，很感谢阿里巴巴中间件团队的徐靖峰，其所写文章带来的启发意义非凡。