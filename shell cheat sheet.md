# Shell Cheat Sheet

## Folder Operations

Delete a directory:`
rm -r directory
`

## CURL

Download file:`
curl -O URLHERE
`

## MySQL

Login:`
mysql -u USERNAME -pPASSWORD
`

Dump:`
mysqldump -u USERNAME -pPASSWORD [database_name] > DUMP.SQL
`

Restore:`
mysql -u USERNAME -pPASSWORD [database_name] < DUMP.SQL
`