# MariaDB Docker image running on Alpine Linux

This Docker image should allow for MariaDB to be used on many
different systems for example amd64, arm64v8, arm32v7.
It is based on
[yobasystems/alpine-mariadb](https://github.com/yobasystems/alpine-mariadb).

## Versions

Uses Alpine 3.12 and the latest mariadb package

## Volumes

| Path                     | Description    |
|:-------------------------|:---------------|
| /var/lib/mysql           | database files |
| /var/lib/mysql/mysql-bin | MariaDB logs   |

## Environment Variables

| Name                | Description                                     |
|:--------------------|:------------------------------------------------|
| MYSQL_DATABASE      | specify the name of the database                |
| MYSQL_USER          | specify the User for the database               |
| MYSQL_PASSWORD      | specify the User password for the database      |
| MYSQL_ROOT_PASSWORD | specify the root password for Mariadb           |
| MYSQL_CHARSET       | default charset (utf8) for Mariadb              |
| MYSQL_COLLATION     | default collation (utf8_general_ci) for Mariadb |
