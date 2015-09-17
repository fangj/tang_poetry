# 全唐诗数据库
爬取的全唐诗数据库

## 在原 hxgdzyuyi 的基础上补充 sqlite 数据库

* 唐诗三百首:	 	tang_300.sqlite 来自[不愿孤独-技术宅也有春天](http://www.mingjianhua.com/post/%E5%94%90%E8%AF%97300%E9%A6%96%E6%95%B0%E6%8D%AE%E5%BA%93access%E7%89%88/SQLite%E7%89%88%E4%B8%8B%E8%BD%BD.html)
* 全唐诗: 		tang_all.sqlite (来自 tang_poetry.sql)

[sql导入到sqlite的折腾过程](sql_to_sqlite.md)

## 使用

1. 新建数据库

```bash
mysql> create database tang_poetry;
mysql> exit;
```

2. 导入数据

```bash
mysql -u root -p -h localhost tang_poetry < tang_poetry.sql
```

## 内容

有两张表，一张作者，一张古诗

## 截图

全唐诗中写诗歌最多的人，以及数量。

![全唐诗中写诗歌最多的人，以及数量。](http://i.imgur.com/Mcwl2TG.png)

杨贵妃的诗歌

![杨贵妃的诗歌](http://i.imgur.com/qgY0SKb.png)
