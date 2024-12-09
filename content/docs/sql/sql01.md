---
date: '2024-12-07T13:46:58+08:00'
draft: true
title: '基础概念'
toc: true
---
## 基础概念
### 什么是⌈数据⌋？
广泛意义来说，任何有用的信息都可以称之为数据。

### 什么是⌈数据库⌋？

> 数据库简而言之就是存储数据的仓库。<br>

数据库（Database，DB）是以一定数据结构组织和存储数据、能够与多个用户共享、具有尽可能小的冗余度、与应用程序彼此独立的数据集合。

### 什么是⌈数据库管理系统⌋？

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
### 什么是⌈关系型数据库管理系统⌋？
关系模型是1970年Edgar F. Codd提出的一种以结构化方式管理数据的方法，而关系型数据库管理系统（RDBMS）是一种基于关系模型的数据库管理系统（DBMS）。

### 数据是如何存储的？

**非关系型数据库**<br/>

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

**关系型数据库**<br/>

在关系型数据库中，数据以表格的形式存储。
| store_id | store_name | address |
|----------|-----------|---------|
| 1        | 门店1     | 地址1    |
| 2        | 门店2     | 地址2    |

## SQL概述
### 什么是⌈SQL⌋？
SQL是Structured Query Language的简称，即结构化查询语言，用于检索和管理关系型数据库中的数据。
### 什么是⌈SQL标准⌋？
为了规范跨数据库产品的SQL语法结构和行为，美国国家标准学会（ANSI）于1986年发布了第一个SQL标准，并在1987年成为国际标准化组织（ISO）标准。
此后，ANSI不断向SQL标准中添加新的功能和命令。
<br/>目前，SQL标准由ANSI和国际标准化组织（ISO）共同维护。

### 什么是⌈SQL方言⌋？
虽然存在SQL标准，但是由于开源社区开发的RDBMS（例如:MySQL和PostgreSQL等开源数据库）不断增加一些ANSI 和 ISO 尚未开发的新特性和功能，导致了SQL代码在不同的数据库管理系统中并不完全具备跨平台性。以下是一些较为流行的SQL方言：
- PL/SQL
- Transact-SQL
- PL/pgSQL
- MySQL