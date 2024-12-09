---
date: '2024-12-07T13:46:58+08:00'
draft: true
title: '基础概念'
toc: true
---

## 什么是⌈数据⌋？
广泛意义来说，任何有用的信息都可以称之为数据。

## 什么是⌈数据库⌋？

> 数据库简而言之就是存储数据的仓库。<br>

数据库（Database，DB）是以一定数据结构组织和存储数据、能够与多个用户共享、具有尽可能小的冗余度、与应用程序彼此独立的数据集合。

## 什么是⌈数据库管理系统⌋？

> 通过数据库管理系统（DBMS）创建和操作数据库。<br>

人们口中常说的“数据库”其实是数据库管理系统（Database Management System，DBMS），数据库管理系统是管理数据库的软件，我们并不直接访问数据库，而是通过DBMS访问和操作数据库中存储的数据。
常见的数据库管理系统：
| 排名 | 数据库管理系统 | 数据库模型       |
|------|--------------|----------------|
| 1    | Oracle       | Relational, Multi-model |
| 2    | MySQL        | Relational, Multi-model |
| 3    | Microsoft SQL Server | Relational, Multi-model |
| 4    | PostgreSQL    | Relational, Multi-model |
| 5    | MongoDB       | Document, Multi-model |
| 6    | Redis        | Key-value, Multi-model |
| 7    | Snowflake     | Relational       |
| 8    | Elasticsearch | Multi-model     |
| 9    | IBM Db2       | Relational, Multi-model |
| 10   | SQLite       | Relational       |
## 什么是⌈关系型数据库管理系统⌋？
关系模型是1970年Edgar F. Codd提出的一种以结构化方式管理数据的方法，而关系型数据库管理系统（RDBMS）是一种基于关系模型的数据库管理系统（DBMS）。

## 数据是如何存储的？
**非关系型数据库**
在非关系型数据库中，数据以键值对的形式存储。
```json
{
    "store_id": 1,
    "store_name": "门店1",
    "address": "地址1",
}
{
    "store_id": 2,
    "store_name": "门店2",
    "address": "地址2",
}
```
**关系型数据库**
在关系型数据库中，数据以表格的形式存储。
| store_id | store_name | address |
|----------|-----------|---------|
| 1        | 门店1     | 地址1    |
| 2        | 门店2     | 地址2    |