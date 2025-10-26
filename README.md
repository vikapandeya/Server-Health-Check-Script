# Server-Health-Check-Script
A full Bash script that performs a comprehensive infrastructure health check on a Linux server. This script will monitor:

⚡ How to Use: Linux_Server

Save script as Linux_Server_health.sh and make executable:

chmod +x Linux_Server_health.sh

./Linux_Server_health.sh


Schedule in cron for automated monitoring (daily at 8 AM):

0 8 * * * /path/to/Linux_Server_health.sh

⚡ How to Use: Multi-Server Health Check & HTML Dashboard

Save script as multi_server_health.sh and make executable:

chmod +x multi_server_health.sh


Ensure SSH key-based access is configured for all servers.

Run manually:

./multi_server_health.sh


Schedule in cron for automated monitoring (daily at 8 AM):

0 8 * * * /path/to/multi_server_health.sh

✅ Features:

Multi-server support: Just add SSH users and IPs to SERVERS.

CPU, Memory, Disk, Swap monitoring with thresholds.

Service check for Nginx, Apache, MySQL.

Top CPU/memory processes for troubleshooting.

Network connections & failed SSH login attempts.

HTML dashboard with color-coded warnings.

Optional email report for admins.

⚡ How to Use: Interactive Multi-Server Health Dashboard (HTML + Graphs)

Save as interactive_dashboard.sh and make executable:

chmod +x interactive_dashboard.sh


Ensure SSH key-based login is configured for all servers.

Run manually:

./interactive_dashboard.sh


Open the dashboard in a browser:

firefox /var/www/html/server_dashboard.html


Schedule in cron (e.g., daily at 8 AM):

0 8 * * * /path/to/interactive_dashboard.sh

✅ Features of This Version:

Interactive visual bars for CPU, Memory, and Disk usage.

Color-coded alerts: red = high usage, green = normal.

Per-server detailed info: uptime, top processes, service status, failed SSH logins, network connections.

Multi-server support: simply add more servers to SERVERS.

Generates a fully browsable HTML dashboard.

Can be scheduled in cron for daily/periodic updates.

Optional email delivery of HTML report.
