# Database Backup and Recovery

- **Backup Command:**
  `mysqldump -u root -p project_db > db_backup.sql`

- **Recovery Command:**
  `mysql -u root -p project_db < db_backup.sql`

- **Execution Steps:**
  1. Created a compressed `.sql` snapshot of the current database.
  2. Simulated a database failure by dropping a test table.
  3. Ran the recovery script to restore all tables and records.
  4. Verified data integrity and row counts.

**Status:** Successfully tested and verified. ✅
