# Laboratory 09: The Cloud Automation Engineer

## Mission Overview

This mission focuses on automating routine cloud operations using Bash scripting and Cron. I created a sample application directory, wrote a backup script to compress its contents, and configured a schedule for automatic backups.

## Objectives

- Understand basic Bash scripting and variables.
- Create and save a script using the nano text editor.
- Modify file permissions using `chmod`.
- Run a script that creates a compressed backup.
- Configure and verify a Cron job.
- Document the automation process in Markdown.

## Commands Executed

```bash
mkdir app-data
echo "This is critical client data." > app-data/data.txt
cat app-data/data.txt
nano backup.sh
./backup.sh
chmod +x backup.sh
./backup.sh
ls -l backups/
crontab -l
env EDITOR=nano crontab -e
```

## Skills Learned

- Creating and executing Bash scripts.
- Using variables to manage directory names and timestamps.
- Compressing files into `.tar.gz` archives.
- Managing file execution permissions.
- Scheduling tasks using Linux Cron.
- Documenting cloud automation tasks in GitHub.