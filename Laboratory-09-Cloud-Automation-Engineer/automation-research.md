# Automation Research

## 1. Bash Script

A Bash script is a file containing a series of commands that the Linux Bash shell executes automatically. The `#!/bin/bash` line, called the shebang, tells the system to use the Bash interpreter to run the script.

## 2. Variables

Variables store values, such as folder paths, that can be reused throughout a script. Using a variable like `$BACKUP_DIR` makes the script easier to maintain because you can change the folder path in one place instead of editing every command that uses it.

## 3. Cron Job

A cron job is a scheduled task in Linux that runs a command or script automatically at a specified time or interval. It is essential for cloud operations because it automates repetitive tasks, such as backups and maintenance, without requiring someone to run them manually.