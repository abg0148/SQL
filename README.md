# Learning SQL 

The Complete course is on BigQuery. 
After creating a sandbox environment run the contents of this initialization script in bigquery worksheet to setup 
tables and schemas for this course.
<details><summary>Initialization Script</summary>
https://github.com/abg0148/SQL/blob/97e6b91779de4799f7274636fbfcab5f8e9a4474/initialization_script.sql#L1C1-L1C1
</details>details>

Check if the setup is correct, by running the following query:
```SQL
SELECT * FROM health.users LIMIT 11;
```

### 1. Selecting All Columns

```SQL
select * from dvd_rentals.language;	
```

### 2. Selecting Specific Columns

```SQL
select language_id, name from dvd_rentals.language;
```

### 3. Limit Output Rows

Always use `LIMIT` to restrict the output to just first few rows from the query

```SQL
select language_id, name from dvd_rentals.language limit 2;
```

### 4. Sorting Query Results
Ordering the result can be done by using `ORDER BY` clause at the end of our queries.
By default, the sorting is done in ascending order and multi-level sorting can be done by specifying more than one column.

- **Sort By Text Column**
