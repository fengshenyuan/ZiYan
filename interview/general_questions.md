# Python
## 为什么Python 3.6以后字典有序并且效率更高？- Python3中的字典是如何实现的？
> entries数组之外，添加了额外的indices数组作为entries的存储索引，使得entries数组从稀疏变得更加紧密，从而节省了空间，提升了遍历的速度，且保证了读取时可以按照插入顺序！

link: https://www.kingname.info/2019/07/13/python-dict/

# SQL 
## SQL之行转列Pivot函数
> Rotates a table by turning the unique values from one column in the input expression into multiple columns and aggregating results where required on any remaining column values. In a query, it is specified in the FROM clause after the table name or subquery.

link:
- https://zhuanlan.zhihu.com/p/76965711 (用case语句实现pivot函数)
- https://docs.snowflake.com/en/sql-reference/constructs/pivot.html

## 数据分析SQL面试题目9套汇总
https://zhuanlan.zhihu.com/p/88942950

## Redis持久化机制：RDB和AOF
> Redis作为一个内存数据库，数据是以内存为载体存储的，那么一旦Redis服务器进程退出，服务器中的数据也会消失。为了解决这个问题，Redis提供了持久化机制，也就是把内存中的数据保存到磁盘当中，避免数据意外丢失
Redis提供了两种持久化方案：RDB持久化和AOF持久化，一个是快照的方式，一个是类似日志追加的方式

作者：TurboSnail
链接：https://juejin.cn/post/6844903939339452430
来源：稀土掘金
著作权归作者所有。商业转载请联系作者获得授权，非商业转载请注明出处。
