## Spark底层最值得一读的论文
- [Resilient Distributed Datasets: A fault-tolerant abstraction for in-Memory cluster computing 原版论文](https://www.usenix.org/system/files/conference/nsdi12/nsdi12-final138.pdf)
- [RDD论文中文翻译版：弹性分布式数据集：基于内存的集群计算的容错性抽象](https://fangmiao97.github.io/2019/04/13/tanslate-Resilient-Distributed-Datasets-A-Fault-Tolerant-Abstraction%E2%80%93for-In-Memory-Cluster-Computing/)
- [入门必读 | Spark 论文导读 - 《Resilient Distributed Datasets: A fault-tolerant abstraction for in-Memory cluster computing》](https://zhuanlan.zhihu.com/p/102572842)
- [Large-Scale Intelligent Microservices](https://arxiv.org/pdf/2009.08044.pdf) - Microsoft paper that presents an Apache Spark-based micro-service orchestration framework that extends database operations to include web service primitives.(跟我说的分布式数据库是一个更好的微服务体系相一致 - 分布式计算的核心范式转换经历了从数据库层不适用 -> 改造服务计算层(to Mircoservice Arch) -> 数据库层适应了分布式与云原生环境(Microservice为核心的架构转换回到以数据库为核心的架构上来) )

## Spark Broadcast Join
Spark Broadcast Join是一种分布式的多计算核心计算方案，这可以在一定程度上扩展spark所能处理的数据规模。shuffle时可以尽可能保证单个节点可以完成运算。这感觉和Snowflake的计算模型不太一样：Snowflake更可能是把数据拉到集群里，然后单个核心直接计算(需要验证？但是怎么验证呢？Snowflake又没有开源 :cry: )

## Spark基础：Parquet
- [Parquet文件存储格式详细解析](https://zhuanlan.zhihu.com/p/363509988)
  - Striping/Assembly算法
    - Repetition Levels
    - Definition Levels
  - Parquet的优势
    - 映射下推(Project PushDown)
    - 谓词下推(Predicate PushDown)
- [一文讲透大数据列存标准格式 - Parquet](https://zhuanlan.zhihu.com/p/341572070)
- [原版论文：Dremel: Interactive Analysis of Web-Scale Datasets](https://storage.googleapis.com/pub-tools-public-publication-data/pdf/36632.pdf)

## Delta Lake
数砖大佬们给 VLDB 投了一篇名为《Delta Lake: High-Performance ACID Table Storage overCloud Object Stores》的论文，并且被 VLDB 收录了，这是第一篇比较系统介绍数砖开发 Delta Lake 的论文
- [全面介绍数砖开发 Delta Lake 的第一篇论文](https://www.sohu.com/a/431026284_315839)
- [Snowflake、Delta Lake 两大新型数仓对比分析](https://zhuanlan.zhihu.com/p/350958074)

## Spark学习路径
- RDD
- RDD之Partition
- Yarn集群运行环境详解
- Spark任务的提交与运行
- Spark Shuffle详解
