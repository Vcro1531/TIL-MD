# SQL JOINS



## Join

###### 둘 이상의 테이블을 연결해서 데이터를 검색하는 방법. 

###### 연결하려면 테이블들이 적어도 하나의 컬럼을 공유하고 있어야 함.

###### Join은 7종류가 있음.(Oracle은 OUTER JOIN이 있지만, MYSQL은 없어서 LEFT+RIGHT조인)



### 1. INNER JOIN : 조인

##### INNER JOIN은 ON 절과 함께 사용되며, ON 절의 조건을 만족하는 데이터만을 가져온다.

```
문법 : 
SELECT * FROM TableA A
INNER JOIN TableB B ON 
A.key = B.key
```

##### 

### 2. OUTER JOIN : 아우터 조인

#### 	-	LEFT OUTER JOIN



# !!알맞은 그림, 제대로 된 내용 전달이 안될듯해 무기한 연기!!



reference : 

https://sql-joins.leopard.in.ua/

https://opentutorials.org/course/3884

https://pearlluck.tistory.com/46

http://tcpschool.com/mysql/mysql_multipleTable_join

https://blog.edit.kr/entry/Left-join-and-Left-outer-join-in-SQL-Server

https://gent.tistory.com/376

https://blog.codinghorror.com/a-visual-explanation-of-sql-joins/