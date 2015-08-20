# MySQL

Login:`
mysql -u USERNAME -pPASSWORD
`

Dump:`
mysqldump -u USERNAME -pPASSWORD [database_name] > DUMP.SQL
`

Restore:`
mysql -u USERNAME -pPASSWORD [database_name] < DUMP.SQL
`

Add user:```
CREATE USER 'newuser'@'localhost' IDENTIFIED BY 'password';
GRANT ALL PRIVILEGES ON * . * TO 'newuser'@'localhost';
FLUSH PRIVILEGES;
```