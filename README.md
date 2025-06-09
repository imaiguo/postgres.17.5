
# PostgreSQL Database Management System


登录PostgreSQL

```bash
> sudo docker run -it --rm postgres:17.5 psql -h 127.0.0.1 -p 2002 -U postgres
>
```


获取自定义配置文件示例

```bash
> sudo docker run -i --rm postgres:17.5 cat /usr/share/postgresql/postgresql.conf.sample > my-postgres.conf
>
```


# Navicat连接postgresql时出现‘datlastsysoid does not exist‘报错的问题

 原因: Postgres 15 从pg_database表中删除了 datlastsysoid 字段引发此错误。
