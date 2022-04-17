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

**Left Outer Join :** It will include the unmatched rows of left side table of the join(left_table **left outer join** right_table)

**Right Outer Join :** It will include the unmatched rows of right side table of the join(left_table **right outer join** right_table)

**Full Outer Join :** It will show both tables unmatched rows.

a)Left Outer Join
select id1,id2,name1,name2
from t11 left outer join t22    [you can omit the keyword outer here]
on id1=id2;

b)Right Outer Join
select id1,id2,name1,name2
from t11 right outer join t22    [again you can omit the keyword outer here]
on id1=id2;

c)Full Outer Join
select id1,id2,name1,name2
from t11 full outer join t22    [as before you can omit the keyword outer here]
on id1=id2;

![Outer Joins](outer-joins.png?raw=true)
