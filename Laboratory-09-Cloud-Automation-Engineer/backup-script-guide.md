# Backup Script Guide

## 1. Backup Script Code

The following Bash script creates a compressed backup of the `app-data` directory. It uses a timestamp in the filename to help distinguish each backup.

```bash
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
```

## 2. File Permissions

The `chmod +x backup.sh` command adds execute permission to the script. This allows Linux to run the script as a program using `./backup.sh`.

## 3. Cron Job Configuration

The Cron expression used for scheduling the backup is:

```bash
0 2 * * * /root/backup.sh
```

This configuration runs the backup script every day at 2:00 AM.

### Breakdown of the Five Time Fields

| Field | Value | Meaning |
|---|---|---|
| Minute | `0` | At minute zero |
| Hour | `2` | At 2 AM |
| Day of Month | `*` | Every day of the month |
| Month | `*` | Every month |
| Day of Week | `*` | Every day of the week |

The final part, `/root/backup.sh`, is the command Cron runs at the scheduled time.