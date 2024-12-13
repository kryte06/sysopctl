# sysopctl Project

## About
*sysopctl* is a custom Linux command-line tool designed to enhance system administration capabilities. 
It provides a unified interface for managing system services, monitoring processes, analyzing logs, and performing system backups. 
This tool simplifies common administrative tasks and improves system resource management.

## Features

**Basic Features:**

*Help Option* 

Command: sysopctl --help

Description: Displays usage instructions and available options.

*Version Information*

Command: sysopctl --version

Description: Shows the current version of the command.

**Intermediate Features**

*List Running Services*

Command: sysopctl service list

Description: Lists all active services, similar to systemctl list-units --type=service.

*View System Load*

Command: sysopctl system load

Description: Displays the current system load averages, akin to the uptime command.

*Manage System Services*

Start a service: sysopctl service start <service-name>

Stop a service: sysopctl service stop <service-name>

Description: Starts or stops a specified service, similar to systemctl start/stop.

**Advanced Features**

*Monitor System Processes*

Command: sysopctl process monitor

Description: Displays real-time process activity, similar to the top command.

*Analyze System Logs*

Command: sysopctl logs analyze

Description: Summarizes recent critical log entries using journalctl.

*Backup System Files*

Command: sysopctl backup <path>

Description: Backs up files from the specified path to the ~/backup/ directory using rsync.

## Usage Instructions

**Prerequisites**

Linux-based environment (e.g., Ubuntu).

**Required tools**

systemctl: For service management.

uptime: To view system load.

top: To monitor processes.

journalctl: For log analysis.

rsync: For backups.

**Setup**

Clone the repository:

git clone https://github.com/kryte06/sysopctl.git

cd sysopctl

Make the script executable:

chmod +x sysopctl

(Optional) Install the manual page:

sudo cp sysopctl.1 /usr/share/man/man1/

sudo mandb

Run Commands

View help: ./sysopctl --help

Check version: ./sysopctl --version

Execute features.

