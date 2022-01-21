# Automatically-start-non-running-service-using-bash

- Save the below script in the /usr/bin or any other directory
- We need to create the script execution permission with chmod. ( chmod +x /usr/bin/service-watcher )

- You can add a schedule according to your accepted downtime or SLA, you can run it every minute as well. To install the above script as a CRON job, run the below command and open it with your preferred editor

- crontab -l | { cat; echo "* * * * *   /usr/bin/service-watcher > /dev/null"; } | crontab -
