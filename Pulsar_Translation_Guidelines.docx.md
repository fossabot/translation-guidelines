Pulsar Translation Guidelines

By Jennifer

请在开始翻译前，我们建议你认真阅读并尽量遵守本文的规范，这会提高你的翻译质量并使你的文章与其他人的风格保持一致。这不仅能减轻校对者校对的工作量，也能使读者阅读起来更加顺畅。

本文为了规范 Pulsar
文档上的术语、用语及规范，在此建立一个供译者、校对者参考的翻译规范和术语表。

**翻译规范**
------------

本规范主要列出了一些常见的翻译问题，并提供了一些指导意见和建议。请译者和校对者尽量遵循本规范，这能使得
Pulsar 中文文档在行为上更统一，在质量上更高。

**1. 翻译地址和翻译文件**

翻译
[https://crowdin.com/project/apache-pulsar/zh-CN\#](https://crowdin.com/project/apache-pulsar/zh-CN)
master/docs 文件夹中的 topics。

**2. 汉字与英文、数字之间需空格**

我们建议汉字与英文或数字之间以空格隔开，以增强中英文混排的美观性和可读性。

注意：中文标点符号前后不需要跟空格，即使前后挨着的是英文单词。

**3. 中文标点符号**

中文里面请使用中文标点符号。注意英文中没有顿号，应该使用顿号的地方在英文中一般使用的是逗号，在翻译时应注意将其翻译为顿号。比如“Kubernetes,
Mesos, Docker” 应该翻译成 “Kubernetes、Mesos、Docker”。

在涉及到多个items时，如果是短语，后面用分号（；）结束，最后一个 item
以句号（。）结尾。

如果每个 item 是个句子，或者已经使用过分号（；），每个 item 以句号结尾。

![](media/9bb9a744708ef4572d7f597575e78672.png)

上面这个例子中，我们建议以句号（。）给每条实践结尾。

**4. 一般用“您”，而不是“你”**

为了风格统一，我们建议使用“您”来称呼。可以不用时，尽量省略不用。

**5. 示例代码及注释**

示例代码中的注释最好能够翻译，当然也可以选择不翻译（当注释很简单时）。

**6. 意译优于直译**

有些同学翻译的文章很容易有翻译腔，就是经常把原文一字不漏地、逐句地翻译了出来。但这样并不代表翻译更准确，反而有时候读着会很别扭。所以建议在翻译完以后，自己多读几遍，看看是否符合原意、是否绕口、是否简洁。在充分理解原文的基础上，可以适当采用意译的方式来翻译。有时候为了简化句子，有些数量词、助词、主语都可以省略。

**...的...的...的...**

比如英文中经常会用 's 来表达从属关系，一字不落地都将其翻译成 "的"
就会很翻译腔。在中文里面有些 "的"
完全可以去掉，不会影响表达的意思，还能简洁很多，看下面的例子：

Pulsar's documentation is located in the docs folder in Pulsar's source code
repository.

当然，你可以将"的"字都翻译出来，但是读起来很不顺畅：

❌ Pulsar 的文档位于 Pulsar 的源码仓库的 docs 文件夹中。

去掉不必要的"的"字，就会简洁很多：

✅ Pulsar 文档位于 Pulsar 源码仓库的 docs 文件夹中。

**一个……**

英文一般比较严谨，当代表多个时，会使用复数名字，在翻译成中文时，一般不需要刻意把这种复数翻译出来。

在英文里，当单数可数名词时，前面一般会有“a”或“an”，但在中文里我们大多数时候是不用把“一个...”给翻译出来的。

比如下面这个例子：

Using a Pulsar client with the proxy

我们可以将“a”翻译成“一个”：

❌ 使用有 proxy 的一个 Pulsar 客户端

虽然看起来没什么问题，但是这里的“一个”完全是多余的，去掉之后不但不会影响翻译效果，而且还会显得更加简洁：

✅ 使用有 proxy 的 Pulsar 客户端

**7. 尽量少用被动句**

英文文档中，有时以物为主语，中文翻译过程中，不需要把“被”字翻译出来。

比如，“...消息被依次分发给消费者...”, 直接翻译成 “消息依次分发给消费者” 即可。

**专业术语**
------------

-   术语翻译表请遵循下方的表格，该表格中列出了社区推荐的翻译，和不推荐翻译的术语。请尽量遵守，但请注意该表格并不是完善的，仍在演进中，如果发现有不恰当的翻译或不确定的翻译，请在邮件列表中讨论，或在这篇
    [Google
    Doc](https://docs.google.com/document/d/1rr2kXGdF9ng9Czpo4ExHyk03t2Pr5gVVrlOTVNuqEN8/edit)
    中评论。

-   **重要：文章中第一次出现专业术语翻译的地方需要给出英文原文。**例如：“使用
    CLI（命令行客户端）...”

-   专有词要注意大小写，如 Pulsar，Java，Scala，API，SQL，不要用小写的 pulsar,
    java, scala, api, sql。

-   当单词是指代码中的属性名、方法名、对象名、类名、标签名等时，可以不译。

### **术语表 （Glossary）**

我们一直认为一个单词一定要结合上下文才能确定准确的含义，所以该表格仅作为翻译的参考。如果遇到不确定的翻译，请随时在社区中发起讨论。

Note：“**CN 翻译”列中仍写原英文的，表示保留英文，不用翻译。**

| **EN Terms**      | **CN 翻译**         | **Note**                                             |
|-------------------|---------------------|------------------------------------------------------|
| Pulsar            | Pulsar              |                                                      |
| message           | 消息                |                                                      |
| topic             | 主题                |                                                      |
| partitioned topic | 分区主题            |                                                      |
| namespace         | 命名空间            |                                                      |
| tenant            | 租户                |                                                      |
| subscription      | 订阅                |                                                      |
| pub-sub           | 发布-订阅           |                                                      |
| producer          | 生产者              |                                                      |
| consumer          | 消费者              |                                                      |
| reader            | 读者                |                                                      |
| cursor            | 游标                |                                                      |
| acknowledged      | 已确认的            |                                                      |
| unacknowledged    | 未确认的            |                                                      |
| retention         | 数据保留            |                                                      |
| retention policy  | 数据保留策略        |                                                      |
| standalone        | standalone          |                                                      |
| cluster           | 集群                |                                                      |
| instance          | 实例                |                                                      |
| broker            | broker              |                                                      |
| proxy             | proxy               |                                                      |
| geo-replication   | 跨地域复制          |                                                      |
| topic lookup      | 主题查找            |                                                      |
| service discovery | 服务发现            |                                                      |
| bookie            | bookie              |                                                      |
| dispatcher        | dispatcher          |                                                      |
| Bookkeeper        | Bookkeeper          |                                                      |
| ledger            | ledger              |                                                      |
| functions         |                     | 取决于语境。如果跟Pulsar Functions一起，建议不翻译。 |
| Pulsar Functions  | Pulsar Functions    |                                                      |
| CLI               | CLI（命令行客户端） |                                                      |
| segment           | 分片                |                                                      |
| hash              | 哈希值              |                                                      |
| key-value         | key-value           |                                                      |
| persistent        | 持久化              |                                                      |
| non-persistent    | 非持久化            |                                                      |
| process guarantee | process guarantee   |                                                      |
| at-most-once      | at-most-once        |                                                      |
| at-least-once     | at-least-once       |                                                      |
| effective-once    | effective-once      |                                                      |
