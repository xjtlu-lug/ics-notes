# CSE103 Final Exam 考点

(Answer is in **bold**)

* The definition of Information System
* foreign key constraint
* odbc (c refers to **connectivity**)
* dbms is interface between **database and program** (From the book "The design of DBMS must take into account the interface between the DBMS and operating system")
* IBM's IMS uses **hierarchical** DBMS
* referential integrity rule applies to **foreign keys**
* QBE(**query by example**)
* Count(\*)
* grouped query (GROUP BY)
* restricting groupings (HAVING clause)
* nested query
* BCNF: if and only if, **every determinant is a candiate key**
* c**reate schema, domain, table, view** (DDL)
* grant (revoke cascade|restrict )
* UML(multiplicity of relation)
* Armstrong’s axiom
  ![](http://static.zybuluo.com/xdx24/hqs6rkljfi87k9nnb9bqp0qi/1.jpg)
* update anomaly
* UK’s 1998 Data Protection Act (**people cannot erase the data**)
* data types
* create database is normalised
* In MS access, input mask is used for **data entry**
* normalisation is a data validation technique
* UML notation, like natural join, selection, projection, etc.
* first develop DB model then process normalization (ch 17.2)
* (jdbc) executeQuery, what does rs.next() do? **Moves the cursor froward one row from its current position**

```java
// answer source: http://docs.oracle.com/javase/6/docs/api/java/sql/ResultSet.html#next%28%29
ResultSet rs = stmt.executeQuery();

rs. next()
```

_Disclaimer: This post is copied from [there](https://www.zybuluo.com/xdx24/note/620867)_
