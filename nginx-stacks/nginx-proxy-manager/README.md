## Nginx Proxy Manager
A manager for Nginx reverse proxies controlled by a web UI

Before deploying, make sure `web_bridge` is set up as a network in Portainer.

There are the `data`, `letsencrypt`, and `mysql` volumes that you do need to keep in mind.

When deploying in Portainer, make sure to add a `stack.env` file for secrets with these variables set:
- `DB_MYSQL_PASSWORD` - Main password for SQL database (from NPM's side), should be the same as `MYSQL_PASSWORD`
- `MYSQL_PASSWORD` - Main password for SQL database (from MariaDB's side), should be the same as `DB_MYSQL_PASSWORD`
- `MYSQL_ROOT_PASSWORD` - Root password for SQL database, can be anything