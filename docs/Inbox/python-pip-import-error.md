---
title: "Python Pip ImportError"
date: 2018-10-21 12:53
---

在Ubuntu中，升级了pip，再次使用 pip 安装相关的 python 包的时候就出现以下错误。
> ImportError: cannot import name main
解决：pip文件在usr/bin目录下，cd进去，进行以下修改

把下面的三行
```python
from pip import main
if __name__ == '__main__':
		sys.exit(main())
```
换成下面的三行
```python
from pip import __main__
if __name__ == '__main__':
		sys.exit(__main__._main())
```
然后问题就解决了。


[@来源](https://blog.csdn.net/accumulate_zhang/article/details/80269313)
