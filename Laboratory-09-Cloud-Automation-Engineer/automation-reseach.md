# Automation Research

## 1. Bash Script

A Bash script is a file that contains commands that Linux can execute in order. The `#!/bin/bash` line, also called the shebang, tells the system to use Bash to run the commands in the file.

## 2. Variables

Variables are used to store information, such as folder paths, that a script needs to use. For example, `$BACKUP_DIR` stores the name or path of the backup folder, making the script easier to update without changing the same path in several places.

## 3. Cron Job

A cron job is a scheduled task in Linux that runs commands or scripts automatically at a specific time or interval. It is useful in cloud operations because it can handle repeated tasks, such as backups, without requiring someone to run them manually every time.