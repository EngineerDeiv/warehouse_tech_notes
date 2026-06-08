You can put `18` or another version. You can verify your PostgreSQL version with:

```bash
postgres --version
```

OR

```bash
postgres -V
```
# stop server PostgreSQL

```bash
sudo systemctl stop postgresql-18
```

# verify the status of the server PostgreSQL

```bash
sudo systemctl status postgresql-18
```

# restart or start the server PostgreSQL

here depends of the version of your database.

```bash
sudo systemctl restart postgresql-18
```