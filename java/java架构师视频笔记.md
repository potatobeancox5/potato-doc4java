#0.名词整理
elk：
edm系统：
swagger2：管理http接口和链接，api文档

todo 翟永超spring-boot教程
spring构建定时任务quartz
幂等性
读写分离
任何主从都有主从延迟

mariaDB 
MariaDB数据库管理系统是MySQL的一个分支，采用GPL授权许可 MariaDB的目的是完全兼容MySQL，包括API和命令行，使之能轻松成为MySQL的代替品
使用XtraDB（英语：XtraDB）来代替MySQL的InnoDB
主从很快
主从延迟解决办法，通过版本号解决
mysql 主从 -> 进程解析binlog 向从节点进行同步
从节点负责读
主节点负责写

sql比较短使用注解比较好
读写分离，使用配置两个数据源，分别注入sqlSessionFactory，还要处理数据源隔离性，
1.定义主从标记
2.隔离线程请求
解决办法使用threadLocal 解决 
