#assignment5
```sql
SELECT * FROM fact;
SELECT * FROM dimension;
CREATE VIEW combined_table AS
SELECT
    f.*,
    d.`region`,
    d.`intermediate-region`,
    d.`region-code`,
    d.`sub-region-code`,
    d.`intermediate-region-code`
FROM
    fact f
INNER JOIN
    dimension d ON f.`country code`= d.`country code`;
    
    
SELECT * FROM combined_table;

```
