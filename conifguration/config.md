---
description: Configuration file format reference
---

# Config File Format

> You should put the "config.yaml" file to the same folder as the main program in.

```Yaml
mode: debug / release
port: your port numble on server
url: your server ip or domain name with the port

# The MySQL database config.
mysql:
  name: your database name
  host: ip or domain name with the port for your mysql.
  username: mysql user
  password: the password of the user
  charset: utf8mb4
```