# Backup Script & Scheduling Guide

## Full Script Code (`backup.sh`)

#!/bin/bash
# Automated Backup Script for CloudNova Technologies

SOURCE_DIR="app-data"
BACKUP_DIR="backups"
TIMESTAMP=$(date +"%Y%m%d_%H%M%S")

echo "Initiating automated backup..."

# Create the backup directory if it does not exist
mkdir -p $BACKUP_DIR

# Compress the source directory into a tarball (.tar.gz)
tar -czf $BACKUP_DIR/backup_$TIMESTAMP.tar.gz $SOURCE_DIR

echo "Backup completed successfully at $TIMESTAMP!"

---

## Understanding chmod +x

By default, newly created text files in Linux are restricted from running as executable programs for security reasons. Running chmod +x backup.sh modifies the file's permission bits, adding (+) execute (x) permissions so the system can run it as an executable script via ./backup.sh.

---

## Cron Schedule Breakdown

The cron expression used to schedule the script:

0 2 * * * /root/backup.sh

Field Breakdown:
1. 0 (Minute): Runs at minute 0 of the hour.
2. 2 (Hour): Runs at hour 2 (2:00 AM in 24-hour format).
3. * (Day of Month): Runs every day of the month.
4. * (Month): Runs every month.
5. * (Day of Week): Runs every day of the week.

Summary: The job executes automatically every single night at exactly 2:00 AM.
