# Description

This docker-compose builds a nextcloud instance including an external database (mariadb) and a database cache (redis).

# How to use this?

1. Edit the ``.env`` file and set the passwords etc.

|variable       |description                            |
|---------------|---------------------------------------|
|MDB_ROOT_PW    |root password for the database         |
|MDB_USER       |database user to connect with          |
|MDB_USER_PW    |password for the database user         |
|MDB_DB_NAME    |name of the database                   |
|REDIS_PORT     |port for the redis instance            |
|NC_ADMIN_USER  |nextcloud admin username               |
|NC_ADMIN_PW    |password for the nextcloud admin user  |

2. Change to this directory and run the following:

```bash
docker-compose up -d
```

3. Open your web browser and navigate to ``<your-ip>:8080``.