#### hadoop
- MR的任务为例讲一下YARN的整个过程
- 实现一个MR，对1T数据全排序
- NameNode的高可用实现
- NameNode高可用中editlog同步过程
- SecondaryNameNode的作用是什么？
- NameNode底层对整个文件系统命名镜像的抽象
- 讲一下HDFS是如何容错，存储信息的？如果用户想hdfs写入数据，请讲一下整个过程？
- 在向HDFS中写数据的时候，当写某一个副本的时候出错怎么处理？
- 谈谈HDFS的读流程？
- 讲一下NameNode中维护的元数据中都存储了哪些信息？
- 讲一下Hadoop与Spark的区别？
- 讲一下Hadoop和YARN中的任务调度算法和任务队列？
- HIVE数据倾斜的原因以及处理办法？Hive的map端聚合为什么能解决数据倾斜？
- 介绍yarn框架？
- Combiner函数的使用发生在那个阶段，以及其使用的条件是什么？Partion的使用阶段？
- 简介HDFS中的接口类型？
- Fsimage与EditLog？
- Fsimage与EditLog合并过程？
- HDFS工具？
- HDFS中在clientProtocol中出现的基本概念的抽象？
- HDFS的ClientProtocol接口
- HDFS的DataNodeProtocol接口
- HDFS的InterDataNodeProtocol接口
- HDFS读数据与写数据
- HDFS源码实现中有哪些优化
- HDFS数据节点的实现
- DataNode流式接口的实现？
- DataXceiver处理读请求？
- DataXceiver处理写请求？
- HDFS写入过程的几种可能？
- HDFS写入过程DataNode出错如何处理（具体过程）？
- 写入过程客户端崩溃怎么处理（租约恢复）？
- HDFS DataNode升级过程？
- HDFS中的distcp与fastcp？
- Hadoop中输入切片inputsplit？
- HDFS NameNode的HA的实现？
- 简述联邦HDFS
- Hadoop如何实现全局排序（阿里）
- HDFS什么时候会出现副本数量多余设定值的情况？
- HDFS如何添加和撤销数据节点？
- 切片？
- 如果避免切片？
- 简述MR的工作机制，以及MR1与MR2的区别？
- MapReduce之间如何选择压缩格式？
- MapReduce的计数器？
- Yarn中的ApplicationMaster故障后如何处理？
- 简述Yarn中的资源调度器？（腾讯，滴滴）
- Hadoop Yarn常见问题以及解决方案
- 浅谈Yarn RM的总体架构（滴滴）
- 浅谈Hadoop Yarn内存和cup的资源调度（管理）和资源隔离机制（百度，cvte）
- 说一下Yarn中AppMaster向ResourceManager申请资源的过程？
- 说一下Hadoop Yarn总的container概念 [资源调度过程]（cvte）
- 简述MR1的不足？
- 简述MapReduce的shuffle机制？
- 简述MapReduce的shuffle机制存在哪些缺陷？
- MapReduce速度较慢？
- Combiner函数何时被使用？
- Reduce函数如何知道从哪台机器获取MapReduce输出？
- Hadoop作用调优？
- 简述Hadoop archive？
- 简述Hadoop对于小文件的处理办法？
- 简述Hadoop的安全认证
- 简述Hadoop如何衡量两个节点之间的拒绝
- HDFS上的副本时怎么放置的
- HDFS的一致性模型
- 简述sqoop

#### Hadoop NameNode源码
1. HDFS的NameNode目录树（NameNode的第一关系管理）[携程]
2. HDFS的NameNode保存镜像文件之后，读取镜像文件的时候，如何判断是目录还是文件？
3. HDFS的NameNode的数据块和数据节点管理（第二关系管理）
4. HDFS数据块副本状态的管理（FSNameSystem）
5. HDFS有一个数据块损坏如何处理？
6. **HDFS有一个数据块，如何知道其副本的情况呢**
7. **客户端在写入数据时只写入一个数据块，如何处理？**
8. **HDFS块的复制？**
9. **HDFS写入的过程？**
10. **HDFS里面怎么建立三副本的过程？**
11. **HDFS删除多余副本的过程（源码）？**
12. HDFS数据块复制时目的节点的饿选择原则（源码）？
13. HDFS删除一个文件的过程（源码）？
14. DataNode删除一个数据块的过程？
15. HDFS客户端删除一个文件是同步还是异步的（源码）？
16. NadeNode中对于数据块的管理？
17. NameNode中的租约管理器？

