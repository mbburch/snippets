# Postgres and SQL Snippets

- To change user and db: `psql -d some_database -U username`

- Restoring from a dump:
  * Change database.yml to point to a new dev database: database-name
  * `rake db:create`
  * `pg_restore --verbose --clean --no-acl --no-owner -h localhost -U dev -d <database-name.dump>`
