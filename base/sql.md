# sql
sql是结构化查询语言的意思，也常用于指关系型数据库。
# 安装mysql
- windows下建议安装XAMPP其包含mysl服务
- linux下自己查各个型号系统的安装方式
- 或者使用docker快速安装
# 创建数据库和表
```sql
-- 创建utf8字符编码的数据库
CREATE DATABASE db_name DEFAULT CHARACTER SET utf8 COLLATE utf8_general_ci;
-- 切换到该数据库下
use db_name;
-- 创建表
create table user(
   id INT NOT NULL AUTO_INCREMENT,
   name VARCHAR(100) NOT NULL,
   age INT NOT NULL,
   PRIMARY KEY ( id )
);
```
# 增删改查
```sql
-- 增
insert into user (name,age) values ('LiMing',22);
-- 查
select * from user limit 10; 
-- 改
update user set age=23 where name='LiMing';
-- 删
delete from user where id = 1;
```
# 常用其他查询
```sql
-- 模糊查询
select * from user where name like '%Li%';
-- 排序
select * from user order by age DESC limit 2;
-- 分组  
select age,count(*) as count from user group by age;
```
# * 扩展了解
- 关联查询join
- IN
- 子查询
- 字符串、时间处理函数
# 扩展学习
非关系型数据库mongodb、redis