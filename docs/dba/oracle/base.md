# oracle 数据库相关操作

> 一些与 `oracle` 相关的数据库操作 `SQL`

## 序列问题
### 1. 查询某个序列的值

```
select sequencename.NEXTVAL from dual;
```

### 2. 删除序列
```
DROP SEQUENCE sequencename;
```

### 3. 更新序列的值
```
create sequence sequencename
  minvalue 1
  maxvalue 999999999999999999999999999
  start with 62
  increment by 1
  cache 20;
```