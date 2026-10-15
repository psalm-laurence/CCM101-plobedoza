# Laboratory 09 - The Cloud Automation Engineer

## Mission Overview

Congratulations! Your ability to secure cloud environments has proven you are ready for the highest 
level of operations. You have been promoted to the Cloud Automation and DevOps Team at CloudNova 
Technologies. 
Up until now, you have been acting as a traditional systems administrator—typing commands manually 
one by one. In large enterprise environments scaling to thousands of servers, manual administration is too slow 
and highly prone to human error. To survive at scale, you must learn to automate. 
Using the KillerCoda Playground, you will step into the role of a Cloud Automation Engineer. You will 
learn the basics of Bash shell scripting, create an automated backup routine, assign executable permissions, and 
configure the Linux Cron scheduler to run your code autonomously.

## Mission Objectives

At the end of this laboratory activity, you should be able to: 
* Understand the fundamental syntax of a Bash shell script, including variables and basic commands. 
* Use a command-line text editor (nano) to write and save executable scripts. 
* Modify Linux file permissions using the chmod command. 
* Understand task scheduling and the syntax of a Linux crontab. 
* Document automation code and Cron job configurations using Markdown. 
* Complete the final chapter of your GitHub Cloud Computing Portfolio.

## Commands Executed

```bash
mkdir app-data
echo "This is critical client data." > app-data/data.txt
cat app-data/data.txt
nano backup.sh
./backup.sh
chmod +x backup.sh
ls -l backups/
tar -tzf backups/backup_*.tar.gz
crontab -l
env EDITOR=nano crontab -e
```

## Skills Learned

Through this activity, I learned how Bash scripts can automate repeated Linux tasks and how variables make scripts easier to maintain. I also learned how to create compressed backups, change file permissions, and schedule commands using Cron. These skills are useful in cloud operations because automation helps make routine administration more consistent and efficient.
