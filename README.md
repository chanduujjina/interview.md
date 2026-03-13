# interview.md


# 1️⃣ What is Indexing in a Database?
## Simple Definition (Best interview start)

- An index is a data structure used to improve the speed of data retrieval operations in a database table

  ### WithOut Index

  ```sql

  SELECT * FROM employee WHERE id = 100;

  ```
### Database must scan the entire table.

```plain text
Full Table Scan
```

### Time Complexity 

``` plain text
O(n)
```
### insex
```sql
CREATE INDEX idx_emp_id ON employee(id);
```
```plain text
        30
      /    \
    10      50
   /  \    /  \
  5   20  40  60
```


### IW
```plain text
Search value
↓
Traverse B-tree
↓
Find node
↓
Get row pointer
↓
Fetch data
```
