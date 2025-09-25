## Apache Guacamole
A way to remotely access other machines via web UI.

Before deploying, make sure `web_bridge` is set up as a network in Portainer.

There is a `guac-db-data` volume that you do need to keep in mind.

When deploying in Portainer, make sure to add a `stack.env` file for secrets with these variables set:
- `MYSQL_ROOT_PASSWORD` - Root password for SQL database, can be anything
- `MYSQL_PASSWORD` - Main password for SQL database, can be anything, but this is what is used mainly