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
