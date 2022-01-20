# Automatically-start-non-running-service-using-bash

You can add a schedule according to your accepted downtime or SLA, you can run it every minute as well. To install the above script as a CRON job, run the below command and open it with your preferred editor

crontab -l | { cat; echo "* * * * *   /usr/bin/service-watcher > /dev/null"; } | crontab -
