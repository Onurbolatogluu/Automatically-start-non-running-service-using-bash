# Automatically-start-non-running-service-using-bash

You can add a schedule according to your accepted downtime or SLA, you can run it every minute as well. To install the above script as a CRON job, run the below command and open it with your preferred editor

sudo crontab -e

* * * * *   /usr/bin/service-watcher > /dev/null

Below are some examples for the crontabs


- 0 */2 * * *   /usr/bin/service-watcher > /dev/null
- 0 0 */1 * *   /usr/bin/service-watcher > /dev/null
- * * * * *   /usr/bin/service-watcher > /dev/null
