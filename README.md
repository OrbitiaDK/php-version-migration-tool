# Fix PHP7.4 -> PHP8 migration

1. Switch between PHP7.4 and PHP8 by editing line 33 in `docker-compose.yml`
2. Put the entire wordpress site into a folder called `wp-site`
3. Put the database as sql-script into a file called `init_db.sql` and save it in the `mariadb` folder
4. Run `docker-compose build php` to update the version
5. Run `docker-compose up` to start the services
