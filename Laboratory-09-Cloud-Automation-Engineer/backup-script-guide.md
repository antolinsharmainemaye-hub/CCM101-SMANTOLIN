# Backup Script Guide

## 1. Overview

This guide explains how to create and schedule an automated backup using a Bash script on Ubuntu. The script compresses the `app-data` directory into a `.tar.gz` archive and saves it in the `backups` directory.

## 2. Backup Script

```bash
#!/bin/bash
# Automated Backup Script for CloudNova Technologies

SOURCE_DIR="app-data"
BACKUP_DIR="backups"
TIMESTAMP=$(date +"%Y%m%d_%H%M%S")

echo "Initiating automated backup..."

mkdir -p "$BACKUP_DIR"

tar -czf "$BACKUP_DIR/backup_$TIMESTAMP.tar.gz" "$SOURCE_DIR"

echo "Backup completed successfully at $TIMESTAMP!"
```

## 3. Making the Script Executable

Run the following command to allow the script to execute:

```bash
chmod +x backup.sh
```

Then run the script:

```bash
./backup.sh
```

The script creates a timestamped compressed backup file inside the `backups` directory.

## 4. Scheduling with Cron

The backup is scheduled to run every day at 2:00 AM using this Cron entry:

```bash
0 2 * * * /root/backup.sh
```

### Cron Schedule Breakdown

- `0` – Minute 0
- `2` – Hour 2 (2:00 AM)
- `*` – Every day of the month
- `*` – Every month
- `*` – Every day of the week

## 5. Verification

Use these commands to verify the backup and Cron schedule:

```bash
ls -lh backups/
crontab -l
```

The first command lists the generated backup archives. The second displays the scheduled Cron jobs.