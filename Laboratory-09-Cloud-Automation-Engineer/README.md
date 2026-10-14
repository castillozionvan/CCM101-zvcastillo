# Laboratory 9: The Cloud Automation Engineer

## Mission Overview
Congratulations! Your ability to secure cloud environments has proven you are ready for the highest level of operations. You have been promoted to the Cloud Automation and DevOps Team at CloudNova Technologies. 

Up until now, you have been acting as a traditional systems administrator—typing commands manually one by one. In large enterprise environments scaling to thousands of servers, manual administration is too slow and highly prone to human error. To survive at scale, you must learn to automate. Using the KillerCoda Playground, you step into the role of a Cloud Automation Engineer to learn Bash shell scripting, create automated backup routines, assign executable permissions, and configure the Linux Cron scheduler to run code autonomously. Remember: *If you have to do a task more than twice in the cloud, you should automate it.*

## Objectives
- Understand the fundamental syntax of a Bash shell script, including variables and basic commands.
- Use a command-line text editor (`nano`) to write and save executable scripts.
- Modify Linux file permissions using the `chmod` command.
- Understand task scheduling and the syntax of a Linux crontab.
- Document automation code and Cron job configurations using Markdown.
- Complete the final chapter of your GitHub Cloud Computing Portfolio.

## Commands Executed

# Create dummy data representing client files
mkdir app-data
echo "This is critical client data." > app-data/data.txt

# Create and edit the backup script
nano backup.sh

# Run script (throws permission denied)
./backup.sh

# Grant execute permissions
chmod +x backup.sh

# Run script successfully and verify output
./backup.sh
ls -l backups/

# Check current active cron jobs
crontab -l

# Edit and install new cron schedule (runs every night at 2:00 AM)
env EDITOR=nano crontab -e
# Added line: 0 2 * * * /root/backup.sh

# Verify installed cron schedule
crontab -l

## Skills Learned
- Writing dynamic shell scripts leveraging variables and command substitution ($(date ...)).
- Managing executable security permissions in Linux with chmod +x.
- Time-based task automation and syntax configuration using the Linux Cron daemon.
- Comprehensive technical documentation and portfolio organization in Markdown.
