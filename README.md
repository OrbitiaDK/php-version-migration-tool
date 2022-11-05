# Fix PHP7.4 -> PHP8 migration

1. Switch between PHP7.4 and PHP8 by editing line 33 in `docker-compose.yml`
2. Put the entire wordpress site into a folder called `wp-site`
3. Put the database as sql-script into a file called `init_db.sql` and save it in the `mariadb` folder
4. Run `docker-compose build php` to update the version
5. Run `docker-compose up` to start the services

## Note:

* Update database configuration in `docker-compose.yml` and `wp-site/wp-config.php`
* Site will be accessible on `localhost:8080`. In some cases, https needs to be disabled by disabling a plugin. It might also be necessary to change site address in the database.
* Database will be accessible on `localhost:33060`.
