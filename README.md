# Server-Health-Check-Script
A full Bash script that performs a comprehensive infrastructure health check on a Linux server. This script will monitor:

⚡ How to Use:

Save script as multi_server_health.sh and make executable:

chmod +x multi_server_health.sh


Ensure SSH key-based access is configured for all servers.

Run manually:

./multi_server_health.sh


Schedule in cron for automated monitoring (daily at 8 AM):

0 8 * * * /path/to/multi_server_health.sh
