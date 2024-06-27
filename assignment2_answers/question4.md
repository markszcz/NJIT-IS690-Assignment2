## Database Management with Alembic and SQLAlchemy

4. **How does Alembic manage database migrations, and why is this important for maintaining database schemas?**
   - Illustrate with an example of a migration script from the project.

Alembic is a datagase migration tool. It specifically is design to work with SQLAlchemy. Alembic gives us a way to manage changes to the database in a structured approach with creating versions. Eeach version would be a schema changed represented by a migration script. Each of these scripts have defined "upgrade()" and "downgrage" functions that represent what is changed in that version's schema.

(venv) markszcz@56k-MainFrame is690_summer2024 % docker compose exec fastapi alembic upgrade head
WARN[0000] /Users/markszcz/Documents/NJIT/IS 690/Assignment2/is690_summer2024/docker-compose.yml: `version` is obsolete 
INFO  [alembic.runtime.migration] Context impl PostgresqlImpl.
INFO  [alembic.runtime.migration] Will assume transactional DDL.
INFO  [alembic.runtime.migration] Running upgrade  -> 6b62f34b7189, initial migration