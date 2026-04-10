# Database Migration: MySQL to PostgreSQL

- **Objective:** Migrating project data while maintaining 100% integrity.
- **Source:** MySQL (Dev Environment)
- **Target:** PostgreSQL (Production Environment)

### Migration Steps:
1. **Schema Conversion:** Mapped MySQL data types to PostgreSQL (e.g., `VARCHAR` to `TEXT`, `DATETIME` to `TIMESTAMP`).
2. **Data Transfer:** Used `pgloader` and custom scripts to move 15,000+ records.
3. **Integrity Check:** Ran row-count validation scripts to ensure zero data loss.
4. **Constraints:** Re-applied Primary Keys and Foreign Keys post-migration.

### Results:
| Table | Source Count | Target Count | Status |
| :--- | :--- | :--- | :--- |
| Users | 1,250 | 1,250 | Verified ✅ |
| Sales | 15,000 | 15,000 | Verified ✅ |
| Projects | 450 | 450 | Verified ✅ |

**Conclusion:** Migration successful with no downtime or data corruption.
