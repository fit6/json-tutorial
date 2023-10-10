# 从零开始的 JSON 库教程

* Milo Yip
* 2016/9/15

也许有很多同学上过 C/C++ 的课后，可以完成一些简单的编程练习，又能在一些网站刷题，但对于如何开发有实际用途的程序可能感到束手无策。本教程希望能以一个简单的项目开发形式，让同学能逐步理解如何从无到有去开发软件。

为什么选择 JSON？因为它足够简单，除基本编程外不需大量技术背景知识。JSON 有标准，可按照标准逐步实现。JSON 也是实际在许多应用上会使用的格式，所以才会有大量的开源库。

这是一个免费、开源的教程，如果你喜欢，也可以打赏鼓励。因为工作及家庭因素，不能保证每篇文章的首发时间，请各位见谅。

## 对象与目标

教程对象：学习过基本 C/C++ 编程的同学。

通过这个教程，同学可以了解如何从零开始写一个 JSON 库，其特性如下：

* 符合标准的 JSON 解析器和生成器
* 手写的递归下降解析器（recursive descent parser）
* 使用标准 C 语言（C89）
* 跨平台／编译器（如 Windows／Linux／OS X，vc／gcc／clang）
* 仅支持 UTF-8 JSON 文本
* 仅支持以 `double` 存储 JSON number 类型
* 解析器和生成器的代码合共少于 500 行

除了围绕 JSON 作为例子，希望能在教程中讲述一些课题：

* 测试驱动开发（test driven development, TDD）
* C 语言编程风格
* 数据结构
* API 设计
* 断言
* Unicode
* 浮点数
* Github、CMake、valgrind、Doxygen 等工具
