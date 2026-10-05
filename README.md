# Problems & Solutions

## Create postgres user + DB
```postgresql
CREATE USER username WITH PASSWORD 'password';
CREATE DATABASE dbname;
GRANT ALL PRIVILEGES ON DATABASE dbname TO username;

-- !!! Switch to DB <dbname>, then continue

GRANT USAGE, CREATE ON SCHEMA public TO username;
```
