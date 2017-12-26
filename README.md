# Shardbatis  mybatis实现数据水平切分的功能

## 介绍：
数据的水平切分包括多数据库的切分和多表的数据切分。目前shardbatis已经实现了单数据库的数据多表水平切分<br>
Shardbatis2.0可以以插件的方式和mybatis3.x进行整合，对mybatis的代码无侵入，不改变用户对mybatis的使用习惯。<br>
shardbatis的使用与原生的mybatis3没有区别，使用者只需要将shardbatis以Mybatis插件的方式引入进来，实现路由策略接口，<br>
实现自己的路由策略即可，此外还需要一个shard_config.xm配置文件，定义哪些sql映射操作需要使用路由策略。<br/>
