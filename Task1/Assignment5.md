I created a script called print.sh that logs the size of the home directory along with the current date and time to diskspace.txt. The script is scheduled to run every 12 hours using a cron job. After at least six entries are recorded, an awk command is used to find and display the line with the maximum size. This solution efficiently automates disk space monitoring and analysis.

