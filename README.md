# SQL Joins

## Table schema
```sql
create table t11(id1 number,name1 varchar2(20));
create table t22(id2 number,name2 varchar2(20));
```


## Inner Join
```sql
select id1,id2,name1,name2
from t11 inner join t22
on id1=id2;
```
We can omit the inner keyword because by default join is inner join. So when you write only join it means inner join.

![Inner Join](inner-join.png?raw=true)

## Outer Joins : Left Outer join, Right Outer Join, Full Outer Join

![Outer Joins](outer-joins.png?raw=true)
