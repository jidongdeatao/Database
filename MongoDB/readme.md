# MongoDB数据库
## 介绍：面向文档的数据库
- 形式
{"id":3,"greeting":"hello,world"}
- 特性
区分大小写 key唯一，不可重复 文档可嵌套 键值对是有序的

- 集合：集合就是一组文档，文档类似关系数据库里的行，集合类似于关系数据库里的表，集合中的文档无需固定的结构(与关系型数据库的区别)
- 集合的命名规范：
  * 1.不能是空字符串("")
  * 2.不能包含\0字符(空字符)
  * 3.不能使用system.的前缀(系统保留)
  * 4.建议不包含保留字"$"
  * 5.用.分割不同命名空间的子集合(如：blog.users, blog.posts)
+ 重点：
  * 1.多个文档组成集合，多个集合组成数据库
  * 2.一个实例可以承载多个数据库
  * 3.每个数据库都有独立的权限
  * 4.保留的数据库名称(admin,local,config)

## 下载与安装
- 详见下载与安装.txt

## 官方文档
https://docs.mongodb.com/

## 基础操作-使用命令行操作数据库
- 参考博客：https://blog.csdn.net/reblue520/article/details/80553377
- 增加数据
- 读取数据
- 修改数据
- 删除数据
- 项目练习：详见-练习任务.txt
## 图形化管理工具-Robomongo
- 官网：https://robomongo.org/
## python操作MongoDB
- 详见：https://github.com/jidongdeatao/Python/tree/master/Python_OperateKu/MongoDB_Operate
