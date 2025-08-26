# Oracle Data Pump Export with Parfile

This module demonstrates how to perform a clean, modular Oracle Data Pump export using a parfile. It’s ideal for DBAs, automation engineers, and certification candidates who want a reusable export workflow.

## 📦 What’s Included

- `parfiles/export_orcl.par`: Parameter file for schema-level export
- `scripts/run_export.sh`: Bash wrapper to execute the export
- `logs/orcl_export.log`: Sample log file (generated after running)

## 🧩 Steps to Use

### 1. Create Oracle Directory Object

```sql
CREATE OR REPLACE DIRECTORY dpump_dir AS '/u01/app/oracle/backups';
GRANT READ, WRITE ON DIRECTORY dpump_dir TO your_user;

