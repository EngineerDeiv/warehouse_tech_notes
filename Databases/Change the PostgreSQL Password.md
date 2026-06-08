# Steps to Change the PostgreSQL Password (postgres User)

## 1. Verify the PostgreSQL Service Status

```bash
sudo systemctl status postgresql
```

(The service was inactive: `"inactive (dead)"`)

## 2. Start/Restart the PostgreSQL Service

```bash
sudo systemctl restart postgresql
```

## 3. Verify the Service Is Running

```bash
sudo systemctl status postgresql
```

(The service is now active: `"active (running)"`)

## 4. Access PostgreSQL as the Superuser (Using Peer Authentication)

```bash
sudo -u postgres psql
```

## 5. Change the Password for the postgres User

```sql
\password postgres
```

(The system will prompt you to enter the new password twice.)

## 6. Exit the PostgreSQL Console

```sql
\q
```