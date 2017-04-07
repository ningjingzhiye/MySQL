# show databases; 显示当前所有的数据库

# create database 名称（character set gbk）; 创建数据库

# drop database 名称; 删除数据库

# use 名称; 使用某个数据库

# 列名称是表中定义的变量名

# 创建表
```
create table students
	(
		id int unsigned not null auto_increment primary key,
		name char(8) not null,
		sex char(4) not null,
		age tinyint unsigned not null,
		tel char(13) null default "-"
	);
```

![](./imgs/01.png)

# show tables; 查看某个数据库有多少个表 
![](./imgs/02.png)

# desc students 查看表结构
![](./imgs/03.png)

# 增 insert into
```
insert into students values(1，"wang", "m", 20, "13811371377");

insert into students(name,sex,age,tel) values("wang2", "w", 21, "13811371371");
```

![](./imgs/04.png)

# 查 select from
```
select * from students;
```
![](./imgs/05.png)

![](./imgs/06.png)

![](./imgs/07.png)

![](./imgs/08.png)

![](./imgs/09.png)

# 删 delete from 表名称 where 删除条件
```
delete from students where id = 2;
```

![](./imgs/10.png)

![](./imgs/11.png)

# 改 update 表名称 set 列名称=新值 where 更新条件;
![](./imgs/12.png)

![](./imgs/13.png)

# 排序 order by      asc（desc）
默认升序

desc是descend 降序意思 

asc 是ascend 升序意思

![](./imgs/14.png)

![](./imgs/15.png)
