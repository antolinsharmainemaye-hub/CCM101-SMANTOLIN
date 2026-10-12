# Mission 9 – Cloud Automation Engineer

## Mission Overview

This mission focuses on automating repetitive cloud operations tasks using Bash scripting and Cron scheduling.

## Objectives

- Understand Bash scripts, variables, and Cron jobs.
- Create a script to back up application data.
- Execute the script and verify the generated backup archive.
- Schedule automatic backups using Cron.

## Commands Executed

```bash
mkdir app-data
echo "This is critical client data." > app-data/data.txt
nano backup.sh
chmod +x backup.sh
./backup.sh
ls -lh backups/
crontab -l
env EDITOR=nano crontab -e
```

## Skills Learned

- Writing and executing Bash scripts.
- Using variables and timestamps in automation.
- Compressing files into `.tar.gz` archives.
- Scheduling recurring tasks using Cron.
- Verifying backup files and scheduled jobs.