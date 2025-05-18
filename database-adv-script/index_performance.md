# Index Performance

## Query
```
-- Before Indexing
EXPLAIN ANALYZE
SELECT * FROM users
WHERE email = 'ernest.wambua@example.com';

-- Create Index
CREATE INDEX idx_users_email ON users(email);

-- After Indexing
EXPLAIN ANALYZE
SELECT * FROM users
WHERE email = 'ernest.wambua@example.com';
```
## Performance Analysis
### With Index
![With Index](with_index.png)

### Without Index
![Without Index](without_index.png)
