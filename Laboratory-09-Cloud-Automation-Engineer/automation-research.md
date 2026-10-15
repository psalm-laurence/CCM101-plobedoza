# Automation Research

## 1. Bash Script

A Bash script is a text file containing commands that the Bash shell executes in sequence to automate tasks. The `#!/bin/bash` line, called the shebang, tells the system to use the Bash interpreter to run the script.

## 2. Variables

Variables store information, such as folder paths, filenames, or timestamps, so the same value can be reused throughout a script. Using a variable like `$BACKUP_DIR` makes the code easier to maintain because I can change the folder path in one place instead of editing every command that uses it.

## 3. Cron Job

A Cron job is a scheduled task in Linux that runs a command or script automatically at a specified time or interval. It is useful in cloud operations because it can automate repetitive tasks, such as backups and maintenance, without requiring someone to run the commands manually each time.
