# Backup Script Guide

## Backup Script

The following Bash script compresses the `app-data` directory into a timestamped `.tar.gz` archive inside the `backups` directory.

```bash
#!/bin/bash
# Automated Backup Script for CloudNova Technologies

SOURCE_DIR="app-data"
BACKUP_DIR="backups"
TIMESTAMP=$(date +"%Y%m%d_%H%M%S")

echo "Initiating automated backup..."

# Create the backup directory if it does not exist
mkdir -p "$BACKUP_DIR"

# Compress the source directory into a tarball (.tar.gz)
tar -czf "$BACKUP_DIR/backup_$TIMESTAMP.tar.gz" "$SOURCE_DIR"

echo "Backup completed successfully at $TIMESTAMP!"
```

## File Permissions

I used the following command to make the script executable:

```bash
chmod +x backup.sh
```

This adds execute permission to `backup.sh`, allowing it to be run as a program using `./backup.sh`.

## Cron Job Configuration

The Cron expression used was:

```cron
0 2 * * * /root/backup.sh
```

This schedules the backup script to run every day at 2:00 AM, using the system's local time.

### Cron Field Breakdown

| Field | Value | Meaning |
|---|---|---|
| Minute | `0` | Run at minute zero |
| Hour | `2` | Run at 2 AM |
| Day of Month | `*` | Every day of the month |
| Month | `*` | Every month |
| Day of Week | `*` | Every day of the week |

The script and schedule automate the backup process, reducing the need for manual intervention. For a production environment, backups should also be checked for errors and stored in a separate location to protect against server failure or data loss.
