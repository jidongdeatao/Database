Redis数据库介绍
用途：数据库、缓存和中间件
类型：
  字符串（strings）
  散列（hashes）
  列表（lists）
  集合（sets）
  有序集合（sorted sets）
  更多。。
  
python操作Redis，详见
https://github.com/jidongdeatao/Python/tree/master/Python_OperateKu/Redis_Operate

Java操作Redis，详见


Redis图形化管理工具：
Redis Desktop Manager
下载及安装：官网：
https://redisdesktop.com/
GitHub：
https://github.com/uglide/RedisDesktopManager
下载地址：
https://redisdesktop.com/download
指导文档：
http://docs.redisdesktop.com/en/latest/


Redis基础操作:
1.字符串(Strings)相关操作
  set -- 设置值
  get -- 获取值
  mset -- 设置多个值
  mget -- 获取多个值
  append -- 添加字符（在后面追加，而不会像get一样会覆盖)
  del -- 删除
  incr/decr -- 增加或减少1
  set key value EX second -- 设置值的过期时间（秒）
  
2.列表（Lists)相关操作
  lpush/rpush -- 从列表的左/右侧添加元素
  llen -- 返回列表的长度
  lrange -- 获取指定长度的列表 （其中0表示列表第一个，1表示列表第二个，以此类推；-1表示列表最后一个，-2表示列表倒数第二个，以此类推）
  lpushx/rpushx -- 从已存在的列表左/右侧添加元素，列表不存在时操作无效
  ltrim -- 只保留指定区间内的元素，不在指定区间之内的元素都将被删除
  （其中0表示列表第一个，1表示列表第二个，以此类推；-1表示列表最后一个，-2表示列表倒数第二个，以此类推）
  lpop/rpop -- 移除最左/最右边的值

3.集合（Sets)相关操作
  sadd/srem -- 添加/删除元素
  sismember -- 判断是否为set的一个元素
  smembers -- 返回该集合的所有成员
  sdiff -- 返回一个集合与其他集合的差异
  sinter -- 返回几个集合的交集
  sunion -- 返回几个集合的并集
  
4.散列（hashes)相关操作
  hset/hget -- 设置/获取散列值
  hmset/hmget -- 设置/获取多对散列值
  hsetnx -- 如果散列已经存在，则不设置
  hkeys/hvals -- 返回所有Keys/Values
  hlen -- 返回散列包含域（field)的数量
  hdel -- 删除散列指定的域（field）
  hexists -- 判断是否存在
