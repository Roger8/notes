#这个是 Python 性能快速优化的第二部分

使用 Map ，Reduce 和 Filter 代替 for 循环 

校验 a in b， 字典 或 set 比 列表 或 元组 更好

当数据量大的时候，尽可能使用不可变数据类型，他们更快 元组 > 列表

在一个列表中插入数据的复杂度为 O(n)

如果你需要操作列表的两端，使用 deque

del - 删除对象使用如下

1） python 自己处理它，但确保使用了 gc 模块

2） 编写 __del__ 函数

3） 最简单的方式，使用后调用 del

time.clock()

GIL(http://wiki.python.org/moin/GlobalInterpreterLock) - GIL is a daemon
