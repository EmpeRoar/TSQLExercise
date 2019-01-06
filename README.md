### TSQLExercise

### Logical Query Processing Order
- 1. FROM
- 2. WHERE
- 3. GROUP BY
- 4. HAVING
- 5. SELECT
- 6. ORDER BY


```sql
SELECT country, YEAR(hiredate) as yearhired, COUNT(*) AS numemployees
FROM HR.Employees
WHERE hiredate >= '20140101'
GROUP BY country, YEAR(hiredate)
HAVING COUNT(*) > 1
ORDER BY country, yearhired DESC;
```
